# The Prompts

Ready-to-paste preference profiles for Claude. Drop one into Settings > Profile > Preferences and Claude stops sounding like a press release.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![For](https://img.shields.io/badge/for-Claude-d97757)
![Templates](https://img.shields.io/badge/templates-50-success)

Two collections live here. The first is 15 modular building blocks you mix and match. The second is 20 complete profiles built around one goal: output that reads like a competent person wrote it, not a model. A third file collects task-specific system prompts, a separate mechanism explained below. Tuned on Opus 4.7, but the mechanics hold across Claude models.

> Two different things, do not confuse them. Personalization preferences (the 15 and 20 files) live in Settings > Profile > Preferences and follow you everywhere. System prompts (the Opus 4.7 file) define one assistant for one job, set through the API or a Claude Project.

## Why this exists

Most prompt collections chase clever one-off tricks. Preferences are a different animal. They run on every message, quietly, so the wins compound and so do the mistakes. A vague preference like "be professional" barely moves the needle. A specific one that names the exact habits you want gone changes the default voice.

The templates here are built for that. They name the AI tells directly: the throat-clearing openers, the empty summaries, the words nobody reaches for in actual conversation. Strip those out and the rest sounds human by subtraction.

## How preferences actually work

Read this before pasting anything. It explains why some lines fire and others sit idle.

- Behavioral preferences (how to respond) only activate when relevant to the task, unless you add a trigger word like "always" or its Indonesian equivalent "selalu". With the trigger, they apply everywhere.
- Contextual preferences (who you are) activate only when the query touches that domain.
- Preferences lose to three things: explicit in-chat instructions, safety, and accuracy. They bias the default. They do not override it.
- There is a character limit. You compose a handful of modules, not all of them.
- Edits apply to new conversations, not the one you are already in.

So "guaranteed 100%" is the wrong frame. Specific and non-conflicting is the right one.

## Quick start

1. Open Settings > Profile > Preferences in Claude.
2. Copy the Core Pack from `templates/20-masterpiece-templates.md`.
3. Paste, save, open a new chat.

That single block covers most of what the 15 modules do. Add a specialist module only when one kind of work dominates your week.

## What's inside

**`templates/15-base-modules.md`**
Fifteen small modules grouped by function: style, intellectual honesty, reasoning, workflow, language. Plus a global base and a composition table. Build your own profile from parts.

**`templates/20-masterpiece-templates.md`**
Twenty complete profiles, one per persona or use case: researcher, engineer, founder, novelist, journalist, analyst, and more. Each one bakes in the anti-slop layer. It closes with a single Core Pack for general use and a universal anti-slop snippet you can bolt onto any profile.

**`templates/opus-4.7-system-prompts.md`**
Fifteen task-specific role prompts for coding, writing, and research, written for how Opus 4.7 reads instructions. Different category from the two files above: these are system prompts for an API call or a Claude Project, not personalization preferences. Adapted with credit from a Chatly blog post; source linked inside.

## The anti-slop layer

This is the spine of both files. Every profile bans the same tells:

- Opener fluff ("great question", "certainly")
- Closer fluff ("hope this helps", "let me know if you have questions")
- Restating your question before answering it
- Summaries that just repeat what was said
- Filler vocabulary (delve, foster, myriad, tapestry, and the rest of the usual suspects)
- Forced rule-of-three phrasing and hollow symmetry
- The em dash, swapped for commas, colons, or periods

It also asks for the harder, positive habits: varied sentence length, a clear position instead of fence-sitting, concrete examples instead of safe abstractions.

## Composing without breaking it

One trap worth flagging. Modules that compress length (brevity, "answer and stop") fight modules that add depth (academic rigor, debate partner). Stack them and they cancel out. Pick one dominant voice, then add narrow specialists on top. The composition tables in each file list combinations that actually work together.

## A note on language

These were written and tested in Indonesian, so the template text is Indonesian-first. The structure ports cleanly. Translate the wording into your language and the mechanics still hold, since the value sits in the instructions, not the vocabulary.

## Disclaimer

Not affiliated with or endorsed by Anthropic. Claude is their product. This is an independent collection of user preferences, nothing more.

## License

MIT. Use them, fork them, ship your own variants. See [`LICENSE`](LICENSE).
