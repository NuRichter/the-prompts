# THE-PROMPTS

Paste-ready preference profiles for Claude. Drop one into Settings, Profile, Preferences, and Claude stops writing like a nervous intern.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![For](https://img.shields.io/badge/for-Claude-d97757)
![Templates](https://img.shields.io/badge/templates-50-success)

Here is the deal. Two collections. The first is 15 building blocks you snap together. The second is 20 finished modules built for one job: writing that sounds like a person who knows the work, not a machine padding for length. A third file holds task-specific system prompts, which is a different tool, and I will say so below so nobody mixes them up. Tuned on Opus 4.7. The mechanics carry across the rest of the lineup.

> Two different things. Do not confuse them. Personalization preferences (the 15 and 20 files) live in Settings, Profile, Preferences and follow you into every chat. System prompts (the Opus 4.7 file) set up one assistant for one job, through the API or a Claude Project. Different box, different effect.

## Why bother

Most prompt collections sell you tricks. Tricks are fun once. Preferences are a different game, because they run on every single message, quietly, every time. So the good ones compound and the lazy ones rot. "Be professional" does nothing. Name the exact habits you want dead, and the default voice actually changes.

These templates do that. They call out the machine tells by name: the throat-clearing openers, the empty summaries, the words nobody says out loud. Cut those, and what is left already reads human. No magic involved. Just subtraction done properly.

## How preferences actually work

Read this before you paste anything. It explains why some lines bite and others just sit there.

- Behavioral preferences (how to respond) only fire when the task calls for them, unless you stamp them with "always" or its Indonesian twin "selalu". Stamp it, and it applies everywhere.
- Contextual preferences (who you are) only fire when the question touches that ground.
- Preferences lose to three things, full stop: a direct instruction in the chat, safety, and being correct. They steer the default. They do not overrule it.
- There is a character limit. You pick a handful, not the whole shelf.
- Edits hit new chats, not the one you are already sitting in.

So "guaranteed 100 percent" is the wrong question. Specific, and not fighting itself, is the right one.

## Start here

1. Open Settings, Profile, Preferences in Claude.
2. Copy the Core Pack from `templates/20-masterpiece-templates.md`.
3. Paste it, save, open a fresh chat. Done.

That one block already does most of what the 15 modules do. Add a specialist only when one kind of work eats your whole week.

## What is in the box

**`templates/15-base-modules.md`**
Fifteen small modules sorted by job: style, intellectual honesty, reasoning, workflow, language. Comes with a global base and a composition table. Build your own profile from parts.

**`templates/20-masterpiece-templates.md`**
Twenty modules aimed squarely at one target: a human voice and the death of AI slop. Grouped into voice, honesty, reasoning, and cross-domain output. Closes with a single Core Pack you can run for anything and a universal anti-slop snippet you bolt onto any profile.

**`templates/opus-4.7-system-prompts.md`**
Fifteen task-specific role prompts for coding, writing, and research, written for how Opus 4.7 reads instructions. Different category from the two above. These are system prompts for an API call or a Claude Project, not personalization preferences. Adapted with full credit from a Chatly blog post. Source linked inside.

## The anti-slop layer

This is the spine of the whole thing. Every profile bans the same tells:

- Opener fluff ("great question", "certainly")
- Closer fluff ("hope this helps", "let me know if you have questions")
- Restating your question before answering it
- Summaries that just chew the same food twice
- Filler vocabulary (delve, foster, myriad, tapestry, the usual crowd)
- Forced rule-of-three and hollow symmetry
- The em dash, swapped for commas, colons, periods

Then it asks for the hard stuff, the part that fakes badly: varied sentence length, a clear position instead of fence-sitting, real examples instead of safe air.

## Mixing them without making a mess

One trap, so pay attention. Modules that squeeze length (brevity, "answer and stop") fight modules that add depth (academic rigor, debate partner). Stack them and they cancel, and you get mush. Pick one voice to lead, then bolt narrow specialists on top. The tables in each file show the combinations that hold together.

## A note on language

Built and tested in Indonesian, so the template text is Indonesian first. The structure travels fine. Translate the words, keep the mechanics, and it still works, because the value sits in the instructions, not the vocabulary.

## Not ours to claim

Not affiliated with Anthropic, not endorsed by them. Claude is their product. This is an independent stack of user preferences. Nothing more, nothing hidden.

## License

MIT. Use them, fork them, ship your own. See [`LICENSE`](LICENSE).
