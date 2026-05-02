# YouTube Scripting Skill

End-to-end YouTube script writing skill for Claude Code, encoding the Iman Gadzhi / Educate.io scripting process documented by Kyle (product team lead at Consulting / Educate.io).

This skill turns Claude into a structured YouTube scriptwriter that walks an operator through the exact same workflow Iman's team uses internally — brief → narratives → outline → context-loaded chat → section-by-section writing → quality gate → trim.

---

## What this skill does

When a user asks Claude (running in Claude Code) to "write a YouTube script", "draft an intro for my video", "script the body points", or any similar request — Claude loads this skill and follows the encoded 10-step workflow:

1. **Preflight** — title, channel, brief, campaign objective, narratives, mechanism+contributor.
2. **Receive brief** — title only / title + bullets / title + meeting transcript.
3. **Confirm narratives** — attention / validation / democratization / timing (channel-modified).
4. **Pick length & depth** (never told to Claude — manual trim later).
5. **Build outline manually** — Intro → Packaging → Body Points → Outro, chronological bullets.
6. **Open fresh Claude chat + paste context prompt** — 3 blocks + the load-bearing "two-three layers deeper / wait for further instruction" closer.
7. **Load reference material** — high-performing transcripts on the same topic + creator's natural-speech transcripts + optional research.
8. **Write section by section** — Intro (One-Sentence Persuasion OR Hook→Break Belief→X-to-X→Credibility) → Packaging (open/close loops) → Body Points (Value Loop: Context → Application → Framing) → Outro. Paste prior approved sections each time.
9. **Quality control gate** — 7-question checklist + banned-language sweep.
10. **Manual length trim** (never ask Claude to shorten).

---

## File layout

```
youtube-scripting/
├── SKILL.md                            # main runbook (Claude reads this when activating)
├── README.md                           # this file
└── reference/
    ├── context-prompt.md               # exact opening prompt template
    ├── narratives-and-channels.md      # 3 channels + 4 narratives explained
    ├── copywriting-structures.md       # both intro structures + packaging loops + Value Loop
    ├── word-tracks.md                  # exact correction prompts for fixing punchy AI output
    ├── banned-ai-language.md           # comprehensive banned-words sweep list
    └── quality-checklist.md            # 7-question gate before finalising
```

---

## Installation

This skill installs into Claude Code's user-skills directory at `~/.claude/skills/`. Once installed, Claude Code automatically loads it whenever a relevant prompt comes in (the description in `SKILL.md` frontmatter is what controls activation).

### Install for the first time

```bash
# Make sure ~/.claude/skills/ exists
mkdir -p ~/.claude/skills

# Clone this repo into the skills folder
cd ~/.claude/skills
git clone https://github.com/laurentickner/youtube-scripting-skill.git youtube-scripting
```

That's it. Claude Code picks up the skill on the next prompt.

### Update to the latest version

```bash
cd ~/.claude/skills/youtube-scripting
git pull
```

### Verify it's loaded

In Claude Code, run:

```
/skill youtube-scripting
```

…or just say *"write a YouTube script for [title]"* and Claude will activate it automatically.

---

## How to share with a teammate

Send your teammate this repo URL: **`https://github.com/laurentickner/youtube-scripting-skill`**

They run the install command above. The skill works the same way for them as it does for you — no per-user config, no API keys, no setup beyond `git clone`.

If they want updates as you improve the skill, they re-run `git pull` whenever they want.

---

## Recommended Claude config when using this skill

- **Model:** Claude Sonnet 4.6 Extended Thinking (the team's tested baseline). Opus only for unusually high-stakes campaigns.
- **One script = one chat.** Never start a new chat partway through. The compounding learning across the conversation is what makes later sections cleaner.
- **Always paste prior approved sections** when requesting the next one.

---

## Source attribution

This skill is a faithful encoding of the YouTube scripting process documented by **Kyle** (product team, Consulting / Educate.io) in the Loom + Notion page covering:

- The 7-part scripting process
- The "two/three layers deeper" Claude-laziness fix
- The peeling-onion correction word-track
- The anti-AI-jargon correction word-track
- The Value Loop body-point framework (originally from creator Callaway)
- The One-Sentence Persuasion intro structure
- The Hook → Break Belief → X-to-X → Credibility intro structure
- The opening / closing retention loops in packaging
- The meet-AND-exceed expectations rule for intros
- The full banned-AI-language list
- The 7-question quality control checklist
- Channel personas (Main / Business / Extended) and how they modify narrative intensity
- The 4 narratives (attention / validation / democratization / timing)
- Unique mechanism + contributor architecture

Credit to Kyle and the Educate.io product team for the underlying playbook.

---

## Maintenance

The skill is versioned in git. To propose an update:

1. Edit the relevant `.md` file in `~/.claude/skills/youtube-scripting/`.
2. `git add . && git commit -m "your update"`
3. `git push`

If your teammate is also using the skill, ping them to `git pull`.
