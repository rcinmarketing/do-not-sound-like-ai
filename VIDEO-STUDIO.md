# Using Tone Studio with Content and Video Studio

[Content and Video Studio](https://github.com/rcinmarketing/content-planning-and-editing) is where you plan and edit short videos. Tone Studio is where you make the words sound like you. They connect in two clicks each way.

## The round trip

1. **In Video Studio**, open a video on the Plan board. Under its script, click **Polish in Tone Studio**. This copies the hook, script, call to action, audience and platforms, and opens Tone Studio.
2. **In Tone Studio**, click **Import from Video Studio**. The script lands in step 2 as "Rewrite a draft", and the rewrite prompt adds video rules: the script is written to be spoken, the first paragraph stays the hook and the last stays the call to action.
3. Work through the steps as usual: rewrite, strip the AI tells, adapt it per platform (TikTok and YouTube Shorts captions are included), and score it.
4. Click **Send to Video Studio** (in the bar at the top, or at the end of step 5).
5. **In Video Studio**, open the same video and click **Paste from Tone Studio**. After you confirm:
   - the hook, script and call to action are replaced with the polished version;
   - each platform version you pasted in step 4 becomes that platform's caption (LinkedIn, Instagram, TikTok, YouTube, X, Substack);
   - your voice profile is saved, and Video Studio's **Send notes to Claude** now includes it, so Claude helps with the video in your voice too.

Nothing is uploaded at any point. Everything moves through your clipboard.

## Where Tone Studio opens from

By default, **Polish in Tone Studio** opens `https://rcinmarketing.github.io/ai-tone-of-voice-prompts/`. If you run Tone Studio somewhere else, set that address once in Video Studio's browser console:

```js
localStorage.setItem('vs.toneUrl', JSON.stringify('http://127.0.0.1:8000/'))
```

## For developers: the card format

The two pages run on different origins and can't read each other's storage, so they swap a plain-text card: a marker line, then one JSON object. Both sides ignore anything they don't recognize, cap every text field at 20,000 characters, and ask before overwriting anything.

**Video Studio → Tone Studio**

```text
VIDEO-STUDIO-CARD v1
{"v":1,"planId":"k3j9x2ab","title":"…","hook":"…","script":"…","cta":"…","audience":"…","pillar":"Authority","platforms":["linkedin","tiktok"]}
```

**Tone Studio → Video Studio**

```text
TONE-STUDIO-CARD v1
{"v":1,"planId":"k3j9x2ab","title":"…","script":"hook\n\nbody\n\ncall to action","hasHook":true,"hasCta":true,
 "captions":{"linkedin":"…","instagram":"…","tiktok":"…","youtube":"…","x":"…","substack":"…"},"voiceProfile":"…"}
```

- `planId` ties the result back to the video it came from. If it doesn't match the open video, Video Studio says so before updating.
- When `hasHook` / `hasCta` is true and the IDs match, the first / last paragraph of `script` goes back into the hook / call to action fields.
- `captions` come from the platform headings in step 4's pasted output (for example `## LinkedIn` or `**TikTok**`).
