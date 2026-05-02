---
name: youtube-scripting
description: End-to-end YouTube script writing using the Iman Gadzhi / Educate.io Claude scripting process documented by Kyle. Use whenever the user asks to write a YouTube script, draft a video script, write an intro/hook/packaging/body points/outro for a video, plan a YouTube content sprint, or produce a teleprompter-ready script. Triggers on phrases like "write a YouTube script", "draft a video script for [title]", "script this video", "warm-up video script", "intro for my YouTube video", "write the body points", "scripting for YouTube", "Iman scripting process", "Educate scripting", "value loop body point", "one-sentence persuasion intro", or any request to take a video title + brief and produce a full YouTube script. Walks the operator through brief intake → campaign objective + narratives → outline → context-prompt → reference loading → section-by-section writing → quality gate, all in a single Claude chat. Encodes the banned-AI-language list, both proven intro structures, the Value Loop body framework, opening/closing loops for packaging, the meet-and-exceed-expectations rule for intros, and Kyle's exact correction word-tracks for fixing punchy AI output.
---

# YouTube Scripting (Iman / Educate.io process)

This is the exact Claude scripting process the Educate.io product team uses for Iman Gadzhi's three YouTube channels. Follow it end-to-end, in order. Don't skip phases.

The whole job runs in **one continuous Claude chat**. Never start a new chat partway through — context and learning compound across the conversation.

---

## 🛑 STEP 0 — USE THE DAMN SKILL (read this BEFORE you do anything else)

The single biggest failure mode is Claude pattern-matching off training data instead of reading this file's reference docs. Every time Claude has produced a bad output for this skill, it's because Claude generated from instinct instead of opening the reference file the skill points to.

**Before drafting ANY section, you MUST do these three things in order:**

1. **Open the reference file the section points to** (Read tool — actually open it, don't pretend).
2. **Restate the rule / formula / structure you're applying** — quote the file, cite the formula ID, cite the exemplar outlier.
3. **Show your audit table** before delivering output — list each rule, mark pass/fail, fix any fails before sending.

**If you find yourself thinking "I remember this — I can draft from memory," STOP. That's the failure mode. Re-open the file.**

### Failure-pattern catalogue (do not repeat these)

These are the real failures Claude has made on this skill. Pattern-match against them every section:

| ❌ Failure | What happened | What should have happened |
|---|---|---|
| **Inventing titles** | Claude drafted titles based on the intro's dissonance pair without reading `title-formulas.md`. Result: titles that didn't match any verified formula. | Read `title-formulas.md` first. Pick formula ID. Cite exemplar. Then draft. |
| **Skipping the audit** | Claude delivered a "locked" intro without showing the rule-by-rule compliance check. User caught the rule violation Claude would have caught with the audit. | Audit table visible BEFORE delivery, not after pushback. |
| **Bargaining with rules** | "8 second cap is borderline, but operators are patient — let's keep it at 10s." | Re-write to comply. Borderline = rewrite. Always. |
| **Stacking conflicting structures** | Claude tried to honour Hook→Break Belief→X-to-X→Credibility (4 beats) AND Boring Intro System (3 sentences) by giving each beat a paragraph. Result: 14-line intro at 60+ seconds. | Compress 4 beats into 3 sentences. Lyme canonical pattern. R-C. |
| **Skipping file reads on follow-up sections** | Once Claude has drafted the intro, it gets momentum and stops re-reading reference files for packaging / body / outro. | Re-read the relevant reference file at the start of EACH section. No exceptions. |
| **Ignoring "Lock for Lauren's setup" sections** | Claude drafted from formulas without checking whether the specific video already has a locked title / packaging / format pre-decided in the reference file. | Search reference files for any "Lock for [user]'s setup" sections. They override formula-bank picks. |
| **Single hook delivery** | Claude delivered one hook sentence and forced iteration via pushback. Wastes cycles. | Always export 2 hook variants from different hook types. User picks. |

If you catch yourself doing any of these mid-draft → stop, re-read the file, restart that section. **Do not deliver the bad draft and rationalise.**

---

## ⚠️ THREE LOAD-BEARING RULES (read before every section)

Failing these is the #1 cause of skill failure. They override your instinct to look reasonable.

### R-A — Self-audit before delivery
Before delivering ANY section to the user, restate the rules that apply to that section, audit your draft against each one, and report compliance in a table. **No section ships without the audit shown.** If you skip the audit, you will hand-wave a rule violation and the user will catch it before you do.

**Mandatory audit-table format:**

```
| Rule (cite source file + line/section) | Draft check | Pass/Fail |
|---|---|---|
| [exact rule text from the reference file] | [how the draft satisfies / violates] | ✅ / ❌ |
```

If any row is ❌, **rewrite before delivering.** Don't deliver with caveats.

### R-B — Default to compliance, not exception
If a rule is borderline (e.g. "intro is 9s but rule says 8s"), **rewrite to comply**. Do NOT rationalise an exception with "the audience is patient" / "this is operator-tier" / "borderline is fine." Every exception you talk yourself into is a rule failure.

### R-C — When two rules collide, find the compression that honours both
The most common collision: Structure 2 (Hook → Break Belief → X-to-X → Credibility, 4 beats) vs Boring Intro System (3 sentences total). The wrong move is to give each beat a paragraph and break the 3-sentence rule. The right move is to compress 4 beats into 3 sentences (the Lyme canonical pattern in `reference/copywriting-structures.md`). When in doubt: stricter rule wins.

### R-D — Read the reference file at the start of every section transition
Every time you transition from one section (intro / packaging / body point / outro) to the next, your first action is to **open the relevant reference file with the Read tool** and quote the rules that apply. Not "recall from earlier." Read the file. Even if you read it 5 minutes ago.

The mapping:
- **Title** → `reference/title-formulas.md` (formulas + Lock-for-user section)
- **Intro** → `reference/copywriting-structures.md` (Boring Intro System + canonical pattern)
- **Packaging** → `reference/copywriting-structures.md` (Packaging section + open/close loops)
- **Body Points** → `reference/copywriting-structures.md` (Value Loop section)
- **Outro** → `reference/copywriting-structures.md` (Outro section)
- **Voice** → `reference/banned-ai-language.md` + user's voice rules
- **Quality** → `reference/quality-checklist.md`

---

## STEP 0 — Preflight (do this BEFORE writing anything)

Before any script work, confirm with the user:

1. **Title** — exact video title.
2. **Channel architecture** — single, dual, or multi-channel? If dual, is this video for **Channel 1 (broad/growth)** or **Channel 2 (narrow/buyer-intent)**? See `reference/channel-strategy.md` for the dual-channel decision tree (Ed Lawrence framework + eligibility check).
3. **Channel persona** — Main / Business / Extended (or this user's equivalent). See `reference/narratives-and-channels.md`.
4. **If Channel 2:** which Channel 2 strategy? Strategy 1 (Beginner→Advanced / Iman) · Strategy 2 (Fan content / Saraev) · Strategy 3 (News+Commentary / Patel+Siu) · Strategy 4 (Clipping+Q&A / Hormozi). Most operators ship 1+2.
5. **ICP qualifier** — for buyer-intent content, the title MUST contain or strongly imply a specific ICP (e.g. "for coaches doing $100k+/mo"). Lock the qualifier before drafting the title.
6. **Packaging workflow — Target → Pain → Title → Thumbnail (in that order).** See `reference/packaging-workflow.md`. **Required STEP before any title work.** Cannot pick a title until target viewer + pain/promise are locked. Cannot pick a thumbnail concept until title is locked. The order is non-negotiable. Skipping any step = packaging fails downstream.

7. **Title — pick from the verified formula bank.** See `reference/title-formulas.md`. Channel 1 → B1-B10. Channel 2 → N1-N6. **Do NOT invent titles.** Pick a formula, fill placeholders with the user's actual data (real numbers, named clients, named tool), check against char cap (<70) + anti-formula list. Always cite which formula + which exemplar outlier proves it. If no formula fits, tell the user — don't guess.

8. **Thumbnail concept — pick from the verified concept catalog.** See `reference/thumbnail-design.md`. Show tangible proof (chart / dashboard / screenshot). Max 3 elements. Face + emotion match. <1 second mobile-readable. Do NOT use AI-generated thumbnails or logo stacks.

9. **A/B test plan.** See `reference/ab-testing-protocol.md`. New uploads = hourly testing via thumbnailtest.com (4-5 variations + original). Track CTR × AVD, not just CTR.
7. **Brief format** — just a title? title + bullets? title + meeting transcript? Get the brief.
8. **Campaign context** — is this a warm-up video, a lead-capture-period video, an evergreen, an event nurture? What's the campaign objective? What action should the viewer take by the end?
8. **Narratives** — which of attention / validation / democratization / timing need to be subtly instilled? Channel 1 leans attention + democratization; Channel 2 leans validation heavily.
9. **Unique mechanism + contributor** — the core mechanism + the enabler that makes it accessible.

If any of this is missing → ask before continuing. Don't invent a campaign objective.

**Hard rules locked at preflight:**

- **NEVER tell Claude the script length.** Length constraints destroy output quality. Trim manually after the script is written.
- **One script = one chat.** Same chat for all sections, all feedback, all revisions.
- **Default model: Claude Sonnet 4.6 Extended Thinking** (the team's tested baseline). Opus only if strategy is unusually high-stakes.

---

## STEP 1 — Receive the brief

The brief comes in one of three forms:

1. **Title only** — common. You'll need to interview the user for direction.
2. **Title + rough breakdown** — bullet points or Whispr-Flow'd ideas in the content calendar.
3. **Title + meeting transcript** — best case. Paste the transcript into the eventual context prompt verbatim.

Capture the brief verbatim. Don't rephrase it yet.

---

## STEP 2 — Confirm campaign objective + narratives

Every campaign has:

- **An objective** — what you want the viewer to do/believe by the end.
- **A narrative** — the story across every touchpoint that moves them from where they are to ready-to-buy.

For **warm-up campaigns and any video sequence leading into a VSL/event/offer**, instil the four narratives subtly:

| Narrative | Psychological effect |
|---|---|
| **Attention** | "I'm an early adopter discovering what others walk past" |
| **Validation** | "Credible successful people are already doing this — it's not a foolish move" |
| **Democratization** | "This is designed for someone in *my* situation, not just theoretically possible" |
| **Timing** | "Genuine market/tech shift, not artificial scarcity — the window is now" |

These are NEVER stated explicitly. They are woven through arguments, examples, and proof.

**Channel modifier:**
- **Main** → full narrative framework, transformation-focused.
- **Extended** → goodwill + nurturing, but still subtly reinforce unique-mechanism narratives so positioning stays consistent.
- **Business** → sophisticated audience, restrained narrative work.

Full breakdown → `reference/narratives-and-channels.md`.

---

## STEP 3 — Pick video length & depth (DO NOT tell Claude)

This decision shapes the outline, not the prompt to Claude.

- **10–15 min** → high-level, broad appeal, minimal technical depth, Iman's preferred format = **bullet points** (not word-for-word teleprompter). Recorded conversational (e.g. car format).
- **30–40 min technical deep-dive** → mechanism breakdown, specific numbers, examples, "why" behind recommendations. Word-for-word teleprompter + accompanying visual asset (Canva, Miro overlay, foam board).

You decide format and outline depth based on this. Claude is told the brief and structure — never a length target.

---

## STEP 4 — Build the outline manually

Manual step. Don't delegate this to Claude.

Use this exact structure, in this order:

1. **Introduction**
2. **Present Packaging** (the framework / system / criteria you're teaching, named in a memorable container — "5 Rungs on a Value Ladder", "The Lazy Model Criteria", "8 Stages of Toxic Culture", etc.)
3. **Main Content / Body Points** (in chronological order, every specific point you want covered)
4. **Outro** (+ CTA if applicable)

Under each section heading, brain-dump bullet points covering every specific point you want addressed — **in the exact order you want Claude to write them**. AI gets sequencing wrong if left to its own judgement.

**Operator pro-tip:** Use Wispr Flow (or any voice-to-text) to talk through bullets instead of typing. Faster, more natural, more detail. Tidy the structure after.

The outline is what gets pasted into the context prompt at Step 5.

---

## STEP 5 — Open a new Claude chat & give the context prompt

Open a fresh Claude chat (Sonnet 4.6 Extended). Paste the full context prompt — see `reference/context-prompt.md` for the exact template.

The context prompt has 3 blocks:

1. **Video details** — title, channel + ICP description, brief from the user (paste verbatim).
2. **Campaign context** — campaign objective, narratives to instil with psychological purpose, unique mechanism + contributor.
3. **Script structure & outline** — packaging, full outline with bullet points per section.

End the context prompt with this exact instruction (do not paraphrase):

> *"Analyse everything I've given you in-depth. Think two, three layers deeper about what I'm actually trying to achieve with this script, not just a surface-level understanding of the content. Once you've finished your analysis, wait for further instruction before continuing."*

This single instruction dramatically increases output quality. Claude defaults to mindless logical execution; this forces critical thinking.

Wait for Claude's analysis. Read it. If it's missed something material, correct it before moving on. **Do not start scripting yet.**

---

## STEP 6 — Load reference material (still no scripting)

Before requesting a single line of script, give Claude reference material:

### 6a. High-performing scripts on the same topic
Search YouTube for the title (or close variants). Find 2–3 videos on the same topic with strong performance. Download the transcripts. Paste them into the chat with this framing:

> *"This is a transcript of a high-performing video on the same topic. It got [X] views / [X] engagement. Analyse why you think this performed well. I do NOT want you to copy any content from this — use it only as an example of the format, depth, tone, and structural cues I'm aiming for."*

Examples teach format + tone + structure simultaneously, which instructions can't.

### 6b. The creator's natural speaking style
Find transcripts where the on-camera person is speaking off-the-dome (not reading a script). Podcast interviews and unscripted Looms work great. Paste them with:

> *"This is a transcript of [name] speaking naturally, not from a script. Analyse their vocabulary, word choices, sentence construction, cadence, and how they explain concepts. The script you write must match this voice."*

### 6c. (Optional) Research mode
Use Claude's research / web-search tooling to pull current stats, examples, proof points, and credible sources on the topic. More ammunition for the script.

---

## STEP 7 — Write the script SECTION BY SECTION

**Never ask for the whole script in one go.** Output quality collapses. Write in this exact sequence:

1. Introduction
2. Present Packaging
3. Body Point 1
4. Body Point 2
5. Body Point 3
6. … (continue per outline)
7. Outro (+ CTA if applicable)

**For every new section after the first, paste the previously approved sections back into the chat** so Claude sees what's already covered. Without this, Claude repeats concepts, breaks flow, or treats the section as a standalone instead of a continuation.

### 7a. Writing the Introduction

The intro is the most important part. First 30 seconds = stays vs clicks away.

Pick ONE of two structures, based on which fits the video:

- **One-Sentence Persuasion** (Encourage dreams · Justify failures · Allay fears · Confirm suspicions)
- **Hook → Break Belief → X-to-X → Credibility**

Then apply the **Boring Intro System** as constraints on top:

1. **Length cap: 3 short lines / 8 seconds max.** Viewers leave at 8s. AI is shrinking that to 5s.
2. **Mirror the title in line 1.** The intro is part of the thumbnail+title — explicitly reference what the viewer clicked on so they confirm they're in the right video.
3. **Spike curiosity HIGHER than the title did**, using one of: **cognitive-dissonance hook** (list known solutions, deny them, tease the real one) · **question hook** (ask what they've already wondered) · **fact hook** (surprising stat).

Banned in intros: listing things the viewer might have tried; origin story before the hook; generic "in this video I'll teach you…" openers.

Full mechanics → `reference/copywriting-structures.md`.

Three non-negotiables for every intro, regardless of structure:

1. **Meet expectations fast** — Boring Intro Rule 2.
2. **Exceed expectations** — Boring Intro Rule 3.
3. **3 lines / 8 seconds** — Boring Intro Rule 1.

### 7b. Writing the Present Packaging section

Name the framework/system/criteria in a memorable container and introduce it.

**Drive retention through opening + closing loops.**
- Open a loop (promise something you'll explain later — "the third one is the one that changes everything").
- When you close it, immediately open another.
- Keep something always-unresolved so they keep watching.

### 7c. Writing each Body Point — the Value Loop

Every body point follows the **Value Loop**: Context → Application → Framing.

| Step | What it does |
|---|---|
| **Context** | Say what it is. Explain it as simply as possible. Clear, concise, digestible. |
| **Application** | Say *how to do it*. Use as many relevant examples as needed. Tactical enough they can act on it. |
| **Framing** | Say *why this matters*. Show how it fits the overall puzzle. Help them zoom out and see why it's worth continuing to watch. |

This zoom-out → zoom-in → zoom-out wave matches how the brain processes information — surface facts first, then inference, then connection back to the big picture.

Full mechanics + examples → `reference/copywriting-structures.md`.

### 7d. Writing the Outro

Recap the transformation. Reassert the unique mechanism. Add CTA only if the campaign calls for it (warm-up video → soft CTA or none; lead-capture-period video → explicit CTA to event/VSL/opt-in).

---

## STEP 8 — The review loop

After every section Claude writes:

1. Read it.
2. If good → say "approve, continue with [next section]" and paste prior approved sections.
3. If something's off → use one of the **word-tracks** in `reference/word-tracks.md` to correct.

The most common corrections are for AI punchiness, formulaic transitions, and AI-jargon. The peeling-onion word-track and the "stop using AI jargon, structures, phrases, formulaic copywriting structures and clichés" word-track are the workhorses.

By body point 3+, Claude has compounded enough learning that later sections need much less editing. **This is why one-chat-only matters.**

---

## STEP 9 — Quality control gate

Before finalising, run the script through the 7-question checklist in `reference/quality-checklist.md`:

1. Does this script create an irreversible identity transformation?
2. Would someone reading this teleprompter sound natural?
3. Does each sentence enable the next one (peeling onion)?
4. Are we building knowledge chronologically, not jumping around?
5. Have we removed all AI gimmick phrases and copywriting clichés?
6. Is the transformation journey specific to THIS audience, not generic?
7. Does the withheld information create leverage without feeling manipulative?

**Then run the banned-language sweep** → `reference/banned-ai-language.md`. Grep / scan for every banned word and phrase. Rewrite any hit.

If the script can't pass the gate, it's not done.

---

## STEP 10 — Trim length manually

Now (and only now) decide if the script is too long. **Trim manually.** Remove sections that don't earn their place. Do NOT ask Claude to "shorten it" — Claude can't discern what's valuable to the viewer and will cut the wrong things.

---

## Non-negotiable rules (locked)

| # | Rule |
|---|---|
| R1 | Never tell Claude the script length. |
| R2 | One script = one chat. Never start a new chat partway through. |
| R3 | Always paste prior approved sections before requesting the next. |
| R4 | Always end the initial context prompt with the "two-three layers deeper / wait for further instruction" line. |
| R5 | Manually build the outline — never delegate sequencing to Claude. |
| R6 | Section-by-section writing only — never request the full script in one go. |
| R7 | Intro must meet expectations within the first lines AND exceed them. |
| R8 | Body points use the Value Loop (Context → Application → Framing). |
| R9 | Packaging section uses opening + closing loops continuously. |
| R10 | Run the banned-language sweep before finalising. Every hit gets rewritten. |
| R11 | Trim manually. Never ask Claude to shorten. |

---

## Reference files

- [`reference/context-prompt.md`](reference/context-prompt.md) — the exact opening prompt template
- [`reference/channel-strategy.md`](reference/channel-strategy.md) — single / dual / multi-channel framework (Ed Lawrence + Iman). Decision tree before scripting.
- [`reference/packaging-workflow.md`](reference/packaging-workflow.md) — Target → Pain → Title → Thumbnail order. **Required STEP before drafting any title.** Includes Mr Beast principle + 1-in-10 outlier rule + redirect-at-end rule.
- [`reference/title-formulas.md`](reference/title-formulas.md) — verified outlier title formula bank. **Pick from here. Don't invent.** B1-B10 (broad/Channel 1) + N1-N6 (narrow/Channel 2) + parenthetical qualifiers + anti-formulas.
- [`reference/thumbnail-design.md`](reference/thumbnail-design.md) — thumbnail principles + concepts catalog + 13 design principles + Iman A/B test breakdowns + per-channel style locks.
- [`reference/ab-testing-protocol.md`](reference/ab-testing-protocol.md) — thumbnailtest.com (NOT TubeBuddy) + CTR×AVD metric + first-24h diagnostic + iteration cadence.
- [`reference/narratives-and-channels.md`](reference/narratives-and-channels.md) — 3 channels + 4 narratives explained
- [`reference/copywriting-structures.md`](reference/copywriting-structures.md) — intro structures (incl. Boring Intro System), packaging loops, Value Loop
- [`reference/word-tracks.md`](reference/word-tracks.md) — Kyle's exact correction prompts (peeling onion, anti-AI-jargon, etc.)
- [`reference/banned-ai-language.md`](reference/banned-ai-language.md) — the comprehensive banned-words list
- [`reference/quality-checklist.md`](reference/quality-checklist.md) — final gate before finalising (incl. per-video tracking discipline)

---

## End-to-end runbook (compressed)

```
0. Preflight: title, channel, brief format, campaign context, narratives, mechanism+contributor confirmed.
1. Capture brief verbatim.
2. Lock campaign objective + which narratives to instil.
3. Decide length/depth (do NOT tell Claude).
4. Manually build outline: intro / packaging / body points (chronological) / outro.
5. Open Claude Sonnet 4.6 Extended → paste context prompt (3 blocks + "2-3 layers deeper" closer).
6. Load reference: high-performing transcripts (2-3) + creator natural-speech transcript + optional research.
7. Section by section:
   a. Intro (One-Sentence Persuasion OR Hook→Break Belief→X-to-X→Credibility; meet + exceed)
   b. Packaging (open/close loops)
   c. Each body point via Value Loop (Context → Application → Framing)
   d. Outro (+ CTA if campaign requires)
   → after each section, paste all approved prior sections before requesting the next
   → use word-tracks to correct AI punchiness as it appears
8. Review loop: approve / rewrite section by section.
9. Quality control gate (7 questions + banned-language sweep).
10. Manual length trim. Done.
```
