<h1 align="center">AI Tone of Voice Prompts</h1>

<p align="center">Copy-paste prompts that make AI write like <b>you</b>, not like a press release.</p>

---

## The problem

You ask an AI to write a LinkedIn post and you get "In today's fast-paced world…", three rocket emojis and the word *delve*. Everyone can spot it now, and readers scroll past.

The fix isn't one magic prompt. It's a short workflow: **capture your voice once, write with it every time, then check the draft for AI tells before you post.**

## Add it to Claude (easiest)

Tell Claude how you sound once, then just say what point you want to make. Claude writes it in your voice, removes the AI giveaways on its own, and gives you a draft for each platform you post on. No API key: it runs on your own Claude plan.

**Claude Code:**

```
/plugin marketplace add rcinmarketing/ai-tone-of-voice-prompts
/plugin install tone-of-voice@rc-in-marketing
```

**Claude.ai or the Claude app:** download [`skills/tone-of-voice`](skills/tone-of-voice) as a ZIP and upload it under **Settings → Capabilities → Skills**.

Then ask: *"Write a post in my voice: I stopped letting AI write my posts and my comments doubled."*

## Or use Tone of Voice Studio

**[Tone of Voice Studio](index.html)** walks you through it in four clicks:

1. **How you sound.** Pick from a few lists, or add your own words. Optional: paste things you've written and video transcripts.
2. **What you want to say.** Just your point.
3. **Your draft**, in your voice. Pick where it will be posted.
4. **A draft for each platform**, ready to copy.

Opened inside Claude, it writes with your own Claude directly. Opened anywhere else, each step opens a new Claude chat with everything filled in, and you paste the reply back. **Download voice kit** saves your voice as `my-tone-of-voice.md`: add it to a Claude Project and every chat writes like you.

**Works with [Content and Video Studio](https://github.com/rcinmarketing/content-planning-and-editing).** Send a video's script over with one click, polish it here, then send the script and a caption for each platform back. See [how the two connect](VIDEO-STUDIO.md).

## The prompts (if you'd rather copy and paste)

| Step | Prompt | What you get | Time |
|---|---|---|---|
| 1 | [Build your voice profile](prompts/01-build-your-voice-profile.md) | A reusable voice profile pulled from your own writing | 10 min, once |
| 2 | [Write or rewrite in your voice](prompts/02-write-in-your-voice.md) | Drafts that sound like you | 1 min per post |
| 3 | [Strip the AI tells](prompts/03-strip-ai-tells.md) | The same draft without the giveaway words and rhythms | 1 min |
| 4 | [Adapt it per platform](prompts/04-platform-adapters.md) | LinkedIn, X, Instagram, email and newsletter versions | 2 min |
| 5 | [Score it before you post](prompts/05-voice-scorecard.md) | A 0–10 "sounds like me" score with line-by-line fixes | 1 min |

Supporting files:

- [`voice-profile-template.md`](voice-profile-template.md): fill this in by hand if you'd rather not use step 1.
- [`ai-tells.md`](ai-tells.md): the words, phrases and patterns that make writing read as AI, and what to say instead.

## How to use it

1. Open [prompt 01](prompts/01-build-your-voice-profile.md), paste in 3–5 things you've written that you're proud of (posts, emails, a talk transcript), and save the voice profile it gives you.
2. In Claude, ChatGPT or Gemini, put that profile in a **Project**, **Custom GPT** or **Gem** so it's loaded every time. No paid plan? Paste it at the top of each chat.
3. Use prompts 02–05 whenever you write.

Works with any modern chat AI. Each prompt has `{{placeholders}}`: replace them, keeping the rest as it is.

## Why it works

- **Examples beat adjectives.** "Friendly but professional" means nothing to a model. Five real paragraphs of yours mean a lot. Step 1 turns your writing into rules *and* examples.
- **Banned lists work best with replacements.** Telling a model "don't say *leverage*" works better when you also tell it what to say instead. [`ai-tells.md`](ai-tells.md) does both.
- **Rhythm gives AI away more than vocabulary.** Same-length sentences, the rule of three, and "It's not X, it's Y" are the real tells. Prompt 03 goes after those, not just the words.

## Before and after

> **Before (default AI):** In today's fast-paced digital landscape, building a personal brand is no longer optional — it's essential. Here are 3 game-changing tips to elevate your presence and unlock new opportunities! 🚀

> **After (with a voice profile):** I posted on LinkedIn for two years before anyone hired me from it. What changed wasn't the posting schedule. I stopped writing what I thought a marketer should say and started writing what I'd tell a friend over coffee.

## More from me

- [Content and Video Studio](https://github.com/rcinmarketing/content-planning-and-editing): plan and edit short-form videos in one browser tab.
- [AI UI/UX Prompts](https://github.com/rcinmarketing/ai-ui-ux-prompts): make AI-built interfaces stop looking AI-built.

Made by Rizza Carla Ramos ([RC in Marketing](https://github.com/rcinmarketing)). Free to use at work, adapt and share under the [MIT License with Attribution Requirement](LICENSE): any copy or version of Tone of Voice Studio must keep the credit footer visible, and shared copies of the prompts or skill must credit RC in Marketing with a link back to this repo.
