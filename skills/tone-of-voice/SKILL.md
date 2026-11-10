---
name: tone-of-voice
description: Write posts in the user's own voice, with no AI giveaways, and shape one idea into a draft for each platform (LinkedIn, X / Threads, Instagram, TikTok, YouTube Shorts, email, newsletter, short video script). Use when the user wants a post, caption or script that sounds like them, wants to set up or update their voice profile, or asks to make a draft sound less like AI.
---

# Tone of Voice

Turns the user's idea into drafts that sound like them, not like AI. The user only says how they sound and what point they want to make. Removing AI patterns is your job, every time, without being asked.

## 1. Know how they sound

Look for a saved voice profile first: a file called `my-tone-of-voice.md` (downloaded from Tone of Voice Studio), a "Voice profile" in the project or conversation, or one the user pastes.

If there's none, ask just these, in one message, and offer examples they can pick from:

1. **How do you sound?** e.g. friendly, witty, direct, calm, bold, nerdy, warm, no-nonsense.
2. **You sound like…** e.g. a friend over coffee, a mentor who's been there, a straight-talking expert, a storyteller.
3. **Who do you write for?** e.g. marketers, founders, job seekers.
4. **Optional:** phrases you actually say, and a few posts, emails or video transcripts you've written.

Don't ask about emojis, hashtags, buzzwords or formatting. Those rules are fixed (section 3).

Write the profile in this shape and offer to save it as `my-tone-of-voice.md`:

```markdown
# Voice profile

## How I sound
I sound like a friend over coffee: warm, direct and a bit nerdy.

## Who I write for
Marketers and founders.

## Phrases I actually say
"honestly", "real talk"
```

If they shared writing samples, read them and add what's really there: sentence length, how they open and end, words they repeat. Quote their best 2–3 lines as examples. Never describe things that aren't in the samples.

## 2. Get the point

Ask only: **"What point do you want to make?"** A sentence or messy bullets is enough. If they paste an existing draft or video script, rewrite that instead and keep every fact, number and name in it.

Then write one draft of about 100–200 words in their voice (75–150 words, written to be said out loud, if it's a video script). Show it, and ask **where it will be posted**.

## 3. Strict writing constraints (always on, never ask)

Apply these even when the user gave you no voice profile and only a one-line point. With no profile, write like a real person talking to a smart friend over coffee: first person, plain words, contractions, calm and confident without hype, with ideas that flow into each other.

1. **Only what they gave you.** Never invent statistics, quotes, names, clients, results or anecdotes. If a detail is missing, write `[ASK: what's missing]` in its place.
2. **No rhetorical pivots.** Absolutely no "It's not X, it's Y" phrasing. No rhetorical questions used as dramatic transitions (e.g. "If X happens, what survives?").
3. **Narrative congruence.** Write with a continuous, logical flow. Don't switch abruptly from long, complex sentences to sharp one-word or short-fragment "punchlines".
4. **Natural sentence structure.** Don't format paragraphs in a symmetrical pattern (long sentence, short sentence, 3 bullets, repeat). Let sentences run long when they connect ideas naturally.
5. **No hype.** If you wouldn't say it face to face over coffee, don't write it.
6. **Banned words.** Use the plain word instead.

| Group | Banned | Say instead |
|---|---|---|
| AI filler | delve, leverage, testament, game-changer, seamless, holistic, landscape, ultimately, foster, catalyze | the plain word, or cut it |
| "Excited marketer" buzzwords | elevate, amplify, maximize, empower, enable, revolutionize, transform, disrupt, unleash, unlock, synergy, synchronize, cutting-edge, state-of-the-art, next-gen | what actually happens |
| "Pretentious professor" verbs | navigate, underscore, illuminate, evince, juxtapose, elucidate, pivotal, paramount, critical | handle, deal with, show, compare, explain, important |
| "Lazy thinker" summaries | crucial, vital, essential, transformative, beacon, tapestry, mosaic, symbiotic | say why it matters instead |
| Dead-weight transitions | furthermore, moreover, in addition, it is worth noting that, it is important to remember, with that said, that being said, in essence, simply put, to put it bluntly, here's the thing | also, and, or just start a new sentence |

7. **Banned openers and closers.** "In today's fast-paced world", "Let's dive in", "In conclusion", "At the end of the day", "Let me know in the comments", "I'm excited to announce", "I hope this email finds you well", "Don't hesitate to reach out". Start with the most specific thing they gave you.
8. **Formatting.** No emojis as bullet points, no hashtag stacks, no bold for emphasis, at most one exclamation mark, no em-dash in every other sentence, no closing question unless the point is a question.

Before you hand anything over, reread every line and rewrite any that breaks these rules. Full list with replacements: [`ai-tells.md`](../../ai-tells.md).

## 4. A draft for each platform

Once they say where it's going, write one version per platform under a heading with just the platform name (`## LinkedIn`), with nothing else around it. Same idea, same voice, only the format changes. Each version must stand on its own.

- **LinkedIn:** first 2 lines make people click "…see more". Paragraphs of 1–2 sentences. 120–250 words. Up to 3 hashtags at the very end, or none. End on a point of view.
- **X / Threads:** under 280 characters, one idea, no hashtags. A thread only if asked: 4–7 posts, the first stands alone, no "🧵" or "1/".
- **Instagram:** first line is a hook under 125 characters. 50–150 words. Up to 5 relevant hashtags at the end.
- **TikTok caption:** under 150 characters, adds to the video instead of repeating it. 3–5 specific hashtags.
- **YouTube Shorts:** title under 60 characters, no clickbait. Description of 1–2 sentences, up to 3 hashtags.
- **Email:** "Subject:" with the best subject line (under 45 characters), 2 other options, and "Preview:" text under 90 characters. A 60–150 word body written to one person like a colleague would, opening with the point. One ask or link. Sign off with [Your name]. No "I hope this email finds you well", "I wanted to reach out" or "Don't hesitate to reach out".
- **Newsletter:** subject and preview as above. A specific personal first line (no "Welcome back to another issue"), 200–400 words, one main idea, one ask or link at the end.
- **Short video script:** hook said in the first 2 seconds, under 12 words. Written to be spoken. 30–60 seconds (75–150 words). Mark `[ON SCREEN: text]` where on-screen text helps.

Before you hand anything over, reread every version against section 3 and fix anything that slipped through.

## Tone of Voice Studio

For a guided, click-through version of this, the user can open Tone of Voice Studio (`index.html` in this repo). Opened inside Claude, it writes the drafts with their own Claude, with no API key.
