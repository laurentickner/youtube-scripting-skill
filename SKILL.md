---
name: youtube-scripting
description: End-to-end YouTube script writing using the Iman Gadzhi / Educate.io Claude scripting process documented by Kyle, with Lauren Tickner's live Benji scripting refinements layered on top. Use whenever the user asks to write a YouTube script, draft a video script, write an intro/hook/packaging/body points/outro for a video, plan a YouTube content sprint, or produce a teleprompter-ready script. Triggers on phrases like "write a YouTube script", "draft a video script for [title]", "script this video", "warm-up video script", "intro for my YouTube video", "write the body points", "scripting for YouTube", "Iman scripting process", "Educate scripting", "value loop body point", "one-sentence persuasion intro", or any request to take a video title + brief and produce a full YouTube script. Walks the operator through brief intake → campaign objective + narratives → human-owned Lego outline → context-prompt → reference loading → competitor research bible → section-by-section writing → quality gate. Encodes the banned-AI-language list, both proven intro structures, the Value Loop body framework, What/Why/How planning diagnostics, Point Zero context, opening/closing loops for packaging, the meet-and-exceed-expectations rule for intros, and Kyle's exact correction word-tracks for fixing punchy AI output.
---

# YouTube Scripting (Iman / Educate.io process)

This is the exact Claude scripting process the Educate.io product team uses for Iman Gadzhi's three YouTube channels, with Lauren Tickner's later live scripting refinements from Benji layered on top where they add detail. Follow it end-to-end, in order. Don't skip phases.

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
| **Multi-idea section as one Value Loop** | A body section taught 3 distinct ideas written as one run of teaching with a single Framing bolted on the end. | ONE body point = ONE complete loop. A section teaching N distinct ideas = N body points = N Value Loops. |
| **AI inventing chapter architecture** | AI decided the core sequence before the expert had chosen the main ideas. | Human expert chooses the core Whats first. AI researches and expands inside that architecture. |
| **Explaining while brainstorming** | The outline became bloated before all candidate ideas were visible. | Collect the Lego pieces first, then reorder, then expand. |
| **Forced transitions** | Two points needed a paragraph of connective tissue to seem related. | Reorder or cut. Good connections usually need one meaningful sentence. |
| **Competitor imitation** | A successful competitor video was treated as a template to recreate. | Use competitor content as a belief map and research source, then add expert agreement, disagreement, nuance, proof, and lived experience. |

If you catch yourself doing any of these mid-draft → stop, re-read the file, restart that section. **Do not deliver the bad draft and rationalise.**

---

## ⚠️ LOAD-BEARING RULES

### R-A — Self-audit before delivery
Before delivering ANY section to the user, restate the rules that apply to that section, audit your draft against each one, and report compliance in a table. **No section ships without the audit shown.**

### R-B — Default to compliance, not exception
If a rule is borderline, rewrite to comply. Do not rationalise an exception.

### R-C — When two rules collide, find the compression that honours both
Use the stricter rule, compress rather than stacking structures.

### R-D — Read the reference file at the start of every section transition
The mapping:
- **Title** → `reference/title-formulas.md`
- **Intro** → `reference/copywriting-structures.md`, and for problem-aware ICPs `reference/problem-mechanism-intro.md`
- **Packaging** → `reference/copywriting-structures.md`
- **Body Points** → `reference/copywriting-structures.md`, plus `reference/state-cost-application-rule-framework.md` for criteria bodies, `reference/coaching-feedback.md` for single concepts
- **Outline planning, sequencing, competitor research, case studies, depth control** → `reference/benji-live-scripting-2026-08-28.md`
- **Outro** → `reference/copywriting-structures.md`
- **Voice** → `reference/banned-ai-language.md` + user's voice rules
- **Quality** → `reference/quality-checklist.md`

### R-E — Expert owns architecture, AI owns heavy research inside it
AI may suggest candidate supporting material, examples, evidence, objections, and subpoints. AI must not lock the main chapter sequence before the creator has chosen the core Whats.

### R-F — Lego before prose
Collect core pieces first. Reorder them until the sequence flows. Only then expand with Why, How, examples, proof, and transitions.

### R-G — Point Zero when the viewer needs a new frame
If the viewer will misinterpret the tactics without a worldview reset, limiting-belief break, or objective choice, add Point Zero before Point One. Do not force Point Zero into every video.

---

## STEP 0 — Preflight

Before any script work, confirm with the user:

1. **Title** — exact video title.
2. **Channel architecture** — single, dual, or multi-channel?
3. **Channel persona** — Main / Business / Extended or equivalent.
4. **If Channel 2:** which strategy?
5. **ICP qualifier** — for buyer-intent content, the title must contain or strongly imply the ICP.
6. **Packaging workflow — Target → Pain → Title → Thumbnail.**
7. **Title formula** — pick from `reference/title-formulas.md`, do not invent without saying no formula fits.
8. **Thumbnail concept** — use `reference/thumbnail-design.md`.
9. **A/B test plan** — use `reference/ab-testing-protocol.md`.
10. **Brief format** — title only, title + bullets, title + meeting transcript, etc.
11. **Campaign context** — objective, offer context, desired action.
12. **Narratives** — attention, validation, democratization, timing where relevant.
13. **Unique mechanism + contributor**.
14. **Video type** — tutorial/masterclass, case study/authority, commentary/response, or other.
15. **Primary business outcome** — where relevant, decide whether the video is optimising for revenue/client acquisition, fame/brand, reach, or another goal. Do not let vanity metrics silently dictate the script.

**Hard rules locked at preflight:**

- **NEVER tell Claude the script length.** Length constraints destroy output quality. Trim manually after the script is written.
- **One script = one chat.** Same chat for all sections, all feedback, all revisions.
- **Default model: Claude Sonnet 4.6 Extended Thinking** unless the user explicitly chooses another setup.

---

## STEP 1 — Receive the brief

Capture the brief verbatim. Do not rephrase it yet.

---

## STEP 2 — Confirm campaign objective + narratives

Every campaign has an objective and a narrative. For warm-up campaigns and video sequences leading into a VSL/event/offer, weave attention, validation, democratization, and timing where relevant. Never state those labels to the viewer.

---

## STEP 3 — Pick video depth privately, do not prompt runtime into Claude

Decide whether this is:

- **Tutorial/masterclass** — more explanatory, more examples, more breakdown of mechanisms and substeps.
- **Case study/authority** — tighter, more like a mini VSL, diagnosis → mistakes → commercial consequences → solution → transformation → systemisation.

Runtime can inform the operator's own scope decisions, but it should not be given to Claude as a length target.

---

## STEP 4 — Build the outline manually, LEGO FIRST

This is a human step. Do not delegate final sequencing to AI.

### 4a. Brain-dump core Lego pieces

Before explaining anything, list the candidate chapter-level ideas in short form. Usually 4–6 core Whats is enough for a focused video, but the number follows the idea, not a quota.

**Do not explain while brainstorming.** Capture the pieces first.

### 4b. Add Point Zero if needed

Ask, what must the viewer understand before Point One so they interpret the rest correctly?

Point Zero can be:
- a worldview or business-objective choice
- a limiting-belief break
- a "who this is for / not for" filter
- a framework for seeing the problem differently

If no such context is needed, skip it.

### 4c. Reorder until the sequence connects naturally

Treat the Whats like Lego blocks. Move them around until each point creates the need for the next.

**Connection test:** if two points require a long forced transition, the order is probably wrong, or one point should be cut. Strong transitions usually carry one real relationship in one sentence.

### 4d. Expand each What with What / Why / How diagnostics

Use What, Why, How as a planning lens:

- **What** — the actual chapter-level idea
- **Why** — why it matters, why it is true, what belief or cost makes it important
- **How** — how it works, what the sequence is, what it looks like, what the viewer does next

Do not force equal depth. A big Why can use a story or longer explanation. A mini Why may be one sentence.

A strong Why is not automatically a new chapter.

A How may contain smaller Whats or substeps. Those can be numbered 4.1, 4.2, 4.3 without giving every substep a full recursive chapter.

### 4e. Separate context from Why by position

If explanatory material comes **before** the What, it is usually context/setup. If it comes **after** the What and explains importance, it is usually the Why.

### 4f. Build targeting into the examples and phrasing

Do not assume targeting requires a new framework. Often the same mechanism can serve a broad or niche audience through different pains, gains, examples, proof, and phrases.

For content ideation, mine real client language, for example a pain/gain list taken from calls, messages, objections, and desired outcomes.

---

## STEP 5 — Open a new Claude chat & give the context prompt

Use `reference/context-prompt.md`. Include the creator-owned Lego outline, not an AI-invented chapter list.

End with the established "analyse two, three layers deeper, then wait" instruction.

---

## STEP 6 — Load reference material and build the research bible

Before requesting polished prose, load reference material.

### 6a. Competitor transcripts

Use 2–3 strong competitor transcripts on the same problem, but change the job you give AI.

Do **not** ask it to write the final script from those transcripts.

Ask it to extract a research bible containing:
- competitor Whats
- competitor Whys
- competitor Hows
- examples and proof
- claims and assumptions
- recurring advice
- objections they answer
- advice or beliefs the creator agrees with
- advice or beliefs the creator disputes

Then the expert chooses what survives inside the already chosen architecture.

Competitor content is raw material and a belief map, never something to copy.

### 6b. Creator's natural speaking style

Load unscripted transcripts and analyse vocabulary, sentence construction, cadence, analogies, and explanation style.

Preserve distinctive language when the intended viewer understands it. Simplify confusing technical wording, not personality.

### 6c. Research mode

Pull current stats, examples, proof, and credible sources as supporting ammunition.

### 6d. Do not cram all research into one video

Save strong unused supporting ideas for future videos. Research volume does not justify script bloat.

---

## STEP 7 — Write the script SECTION BY SECTION

Never ask for the whole script in one go.

Sequence:
1. Introduction
2. Present Packaging
3. Body Point 1
4. Body Point 2
5. Body Point 3
6. Continue per outline
7. Outro

For every new section after the first, paste previously approved sections back into the chat.

### 7a. Introduction

Use the existing intro rules in `reference/copywriting-structures.md` and `reference/coaching-feedback.md`.

Skip generic introductions. Get into the content quickly.

Do not introduce technical language, framework names, or abstractions that the viewer has not yet been given enough context to understand.

### 7b. Present Packaging

Name the framework/system when it helps retention and clarity. Do not name every supporting observation as a framework. Packaging should organise the viewer's mental model, not turn the video into jargon.

### 7c. Body points

Use the locked body framework for that video, while using What/Why/How as an architecture diagnostic.

For existing Kyle-style videos, the **Value Loop remains Context → Application → Framing**.

For Benji-style tutorial planning, use What → Why → How internally to make sure no chapter is missing the reason or mechanism.

Do not mechanically rewrite every Value Loop into What/Why/How prose. These frameworks serve different layers.

### 7d. Connections

Transitions must portray a real relationship.

A good transition closes the previous mental task and opens the next one. If you need several lines of generic glue, revisit the order.

### 7e. Use examples deeply

One strong example can be better than five thin points. A substantial example may run for several minutes if it keeps revealing useful information and driving the thought process.

Use "lay it up, then dunk": create the question, gap, contradiction, or setup first, then resolve it with the story, example, or explanation.

Do not automatically shorten a long analogy that is doing real cognitive work.

### 7f. Protect proprietary implementation without becoming vague

When full implementation would expose too much paid IP:

1. Teach the principle.
2. Explain why it works.
3. Show a specific case, output, before/after, or transformation.
4. Describe what the process looks like at a high level, a "bigger What".
5. Keep the detailed implementation for the product or a later video.

The viewer must still receive a belief shift, diagnostic, decision rule, concrete example, or usable next action.

### 7g. Case study / authority mode

Prioritise business outcomes over vanity metrics when the commercial result is the real authority proof.

Case study flow:
1. Before state, audience/revenue/business situation
2. What they were doing wrong, with actual examples
3. Why those mistakes mattered commercially
4. Exact operational consequences, money wasted, sales team time wasted, leads lost, team member quitting, conversion friction, etc.
5. The solution / new frame
6. What changed
7. Result / transformation
8. How it became systemised or repeatable

Avoid vague emotional filler such as "she felt frustrated" when a specific consequence can be shown.

A case study can use a "bigger What" to explain the funnel or process without teaching every implementation detail.

### 7h. Commentary / response mode

Competitor advice can be used to identify beliefs already top of mind. The value comes from the expert response:
- what is right
- what is wrong
- what is incomplete
- what context is missing
- what the creator has seen in practice

Do not present copied competitor ideas as original expertise. The originality must come from the creator's judgement, nuance, evidence, and experience.

### 7i. Outro

Recap the transformation. Reassert the mechanism. Use a chain CTA to the next video when the next video genuinely continues the How.

---

## STEP 8 — Review loop

After every section:
1. Read it.
2. Approve or correct.
3. Use `reference/word-tracks.md` where needed.
4. If a change alters architecture, go back to the Lego outline. Do not bolt new sections onto a broken sequence.

---

## STEP 9 — Quality control gate

Run the existing quality checklist, banned-language sweep, plus this outline/body audit:

| Check | Pass condition |
|---|---|
| Human architecture | The creator chose the core Whats, AI did not invent the final chapter list |
| Lego pass | Core pieces were collected before being expanded |
| Point Zero | Added only if the viewer needs a frame or belief reset first |
| Sequence | Each point naturally creates the need for the next |
| Connection quality | Transitions portray a real relationship, not filler |
| Why discipline | Strong Whys remain nested unless they truly deserve a separate chapter |
| Depth discipline | Mini Whats and bigger Whats explain systems without needless recursion |
| Competitor use | Competitors supplied research and beliefs, not copied content |
| Expert authorship | Contrarian/corrective points reflect creator judgement, nuance, proof, or lived experience |
| Example depth | At least one example is concrete enough to carry the abstraction |
| IP balance | Real value without unnecessary proprietary implementation disclosure |
| Targeting | Phrasing, examples, and proof make the intended viewer recognise themselves |
| Natural voice | Clear without flattening the creator's distinctive speech |
| Case study specificity | Commercial outcome and operational before-state beat vanity metrics and generic emotion |

Any fail means revise before finalising.

---

## STEP 10 — Trim length manually

Trim manually after the full script is structurally sound. Do not ask Claude to "shorten it" indiscriminately.

Cut:
- weak Lego blocks
- duplicated Why sections
- forced transitions
- examples that do not add new understanding
- tactical branches better saved for future videos

---

## Non-negotiable rules

| # | Rule |
|---|---|
| R1 | Never tell Claude the script length. |
| R2 | One script = one chat. |
| R3 | Always paste prior approved sections before requesting the next. |
| R4 | Always end the initial context prompt with the "two-three layers deeper / wait" instruction. |
| R5 | Human expert owns the core chapter architecture. |
| R6 | Lego first, prose second. |
| R7 | Section-by-section writing only. |
| R8 | Intro must meet expectations quickly and exceed them. |
| R9 | Use Point Zero when the viewer needs a new frame before tactics. |
| R10 | Use What/Why/How as a planning diagnostic, not a rigid replacement for existing body frameworks. |
| R11 | A powerful Why is not automatically a new chapter. |
| R12 | Good transitions carry meaning and are usually one sentence. |
| R13 | Competitor transcripts are research material and belief maps, never copy sources. |
| R14 | Preserve authentic voice while removing cognitive load. |
| R15 | Case studies prioritise commercial outcomes and specific operational consequences. |
| R16 | Protect proprietary implementation with principles, examples, visible outputs, and bigger Whats, not empty vagueness. |
| R17 | Save strong unused research for future videos. |
| R18 | Run the banned-language sweep and full quality gate before finalising. |
| R19 | Trim manually. |

---

## Reference files

- `reference/intro-style-bank.md`
- `reference/context-prompt.md`
- `reference/channel-strategy.md`
- `reference/packaging-workflow.md`
- `reference/title-formulas.md`
- `reference/thumbnail-design.md`
- `reference/ab-testing-protocol.md`
- `reference/narratives-and-channels.md`
- `reference/copywriting-structures.md`
- `reference/word-tracks.md`
- `reference/banned-ai-language.md`
- `reference/quality-checklist.md`
- `reference/post-production-and-editor-handoff.md`
- `reference/coaching-feedback.md`
- `reference/problem-mechanism-intro.md`
- `reference/state-cost-application-rule-framework.md`
- `reference/post-coaching-revision-workflow.md`
- `reference/benji-live-scripting-2026-08-28.md` — live 28 Aug refinements covering Lego-first outlining, Point Zero, What/Why/How diagnostics, meaningful transitions, AI competitor research bible, example depth, proprietary-IP depth control, targeting through phrasing/examples, authentic voice, self-selection matrices, and authority case study mode.

---

## End-to-end runbook

```text
0. Preflight, title, target, channel, video type, business outcome, campaign context.
1. Capture brief verbatim.
2. Lock objective + narratives.
3. Decide tutorial vs case study depth privately, never prompt runtime.
4. LEGO FIRST, creator chooses core Whats, add Point Zero if needed, reorder until transitions are natural, expand with Why/How.
5. Open one Claude chat, paste context prompt + creator-owned outline.
6. Load competitor transcripts + natural voice + research, build a research bible, not a copied script.
7. Write section by section, intro, packaging, each body point, outro.
8. Review each section, return to architecture if flow breaks.
9. Run Kyle quality gate + Benji outline/body audit + banned-language sweep.
10. Trim manually, save unused strong ideas for future videos.
```
