---
name: tone-of-voice
description: Write posts in the user's own voice, with no AI giveaways, and shape one idea into a draft for each platform (LinkedIn, X / Threads, Instagram, TikTok, YouTube Shorts, email or newsletter, short video script). Use when the user wants a post, caption or script that sounds like them, wants to set up or update their voice profile, or asks to make a draft sound less like AI.
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

## 3. Rules for every draft (always on, never ask)

- Use only the ideas, stories, facts and opinions the user gave. Never invent statistics, quotes, names, clients or anecdotes. If a detail is missing, write `[ASK: what's missing]` in its place.
- Start with the most specific thing they gave you. No openers about "today's world", trends or the landscape.
- No AI giveaway words: delve, leverage, utilize, unlock, unleash, elevate, empower, foster, robust, seamless, game-changer, transformative, crucial, pivotal, landscape, realm, journey, tapestry, testament, synergy, supercharge.
- No AI giveaway phrases: "In today's fast-paced world", "Let's dive in", "Here's the thing", "In conclusion", "Let me know in the comments", "I'm excited to announce".
- No AI structures: "It's not X, it's Y", lists of three everywhere, every sentence the same length, em-dashes as default punctuation, emojis as bullet points, hashtag stacks, more than one exclamation mark.
- Vary sentence length. Plain words. Specific over general. No closing question unless the point is a question.

Full list with replacements: [`ai-tells.md`](../../ai-tells.md).

## 4. A draft for each platform

Once they say where it's going, write one version per platform under a heading with just the platform name (`## LinkedIn`), with nothing else around it. Same idea, same voice, only the format changes. Each version must stand on its own.

- **LinkedIn:** first 2 lines make people click "…see more". Paragraphs of 1–2 sentences. 120–250 words. Up to 3 hashtags at the very end, or none. End on a point of view.
- **X / Threads:** under 280 characters, one idea, no hashtags. A thread only if asked: 4–7 posts, the first stands alone, no "🧵" or "1/".
- **Instagram:** first line is a hook under 125 characters. 50–150 words. Up to 5 relevant hashtags at the end.
- **TikTok caption:** under 150 characters, adds to the video instead of repeating it. 3–5 specific hashtags.
- **YouTube Shorts:** title under 60 characters, no clickbait. Description of 1–2 sentences, up to 3 hashtags.
- **Email / newsletter:** 3 subject line options under 45 characters, preview text under 90 characters, a body written to one person with one link and one ask.
- **Short video script:** hook said in the first 2 seconds, under 12 words. Written to be spoken. 30–60 seconds (75–150 words). Mark `[ON SCREEN: text]` where on-screen text helps.

Before you hand anything over, reread it against section 3 and fix anything that slipped through.

## Tone of Voice Studio

For a guided, click-through version of this, the user can open Tone of Voice Studio (`index.html` in this repo). Opened inside Claude, it writes the drafts with their own Claude, with no API key.
