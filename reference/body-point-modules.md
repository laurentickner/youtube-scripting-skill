# Body-Point Modules — Modular Script Composition

How to compose scripts by mixing and matching reusable **body-point frameworks** studied from top creators, filled with the user's own content in the user's own voice.

This is the system behind the `template-bank/` (lives in the working project folder, e.g. `Desktop/youtube-strategy/template-bank/`). This file is the METHOD; the bank is the LIBRARY.

---

## The principle (read first)

A body point is not a paragraph of text. It's a **structural framework** — a shape with a function, an entry/exit register, slot points where content goes, and rules for what it can sit next to.

You study how proven creators build body points, extract the SHAPE (not their words), and recombine shapes from different videos to compose new scripts.

**Worked example — a "3 methods" video:**
- Method 1 body point uses the `numeric-walkthrough` shape (studied from Creator A's video)
- Method 2 body point uses the `contrast-pair` shape (studied from Creator B's video)
- Method 3 body point uses the `mini-case-study` shape (studied from Creator C's video)

Three different structural shapes, combined into one original script, each filled with the user's own examples / numbers / claims in the user's own voice.

**The line (non-negotiable):**
- ✅ Reuse the SHAPE — the function, the beat skeleton in structural verbs, the slot specs, the rhythm pattern.
- ❌ Never reuse the creator's actual SENTENCES with the nouns swapped out. That reproduces their copyrighted script and makes the user sound like the creator, not themselves. It also fails the user's own coach's #1 rule: sound natural, like you, zero trace.
- The test: could a stranger reconstruct the creator's original lines from the module? If yes, it's too verbatim — strip it back to function.

---

## Module schema

Each body-point module is a standalone file with these fields:

```
MODULE ID: <creator>-<template>-<position>-<shape>

SHAPE: <controlled-vocab shape name>
ROLE: <what job it does in a script>
FUNCTION (one sentence): <what this module accomplishes>

BEAT SKELETON (structural verbs only — NO creator text)
1. <function of beat 1>
2. <function of beat 2>
...

LENGTH NORM: <seconds / words / beat count>

ENTRY REGISTER REQUIRED: <energy + tone the script must be in to enter this module>
EXIT REGISTER DELIVERED: <energy + tone the module leaves the script in>

REQUIRES (dependency contract): <what must be true upstream — e.g. "abstract claim already named", "a loop already open">
PROVIDES: <what this module delivers downstream — closes a loop / names a principle / shifts energy>

LOOP INTERACTION: <opens / closes / neutral + loop namespace>

SLOT SPECS (what content the user brings)
- Beat N: <SLOT TYPE> — <length + constraint>

CASE-STUDY FIT: <which of the user's real assets fit which slot>

COMPATIBILITY
- compatible-after: [shapes this can follow]
- incompatible-after: [shapes that collide if placed before this]
- compatible-before: [shapes this can lead into]
- incompatible-before: [shapes that collide if placed after this]

PORTABILITY: <standalone | requires-setup | requires-callback>

NOTES: <when to reach for it, gotchas, pairing tips>
```

See `template-bank/<creator>/modules/` for fully-built examples.

---

## Shape taxonomy (controlled vocabulary)

Body points get indexed by SHAPE so you can browse "I need a `mechanism-reveal` here" across every creator at once. Current shapes:

| Shape | What it does | Best slot type |
|---|---|---|
| `enumerated-steps` | numbered process, step 1 → step N → synthesis | CLAIM per step |
| `contrast-pair` | wrong-way vs right-way reframe | SYMPTOM + RULE |
| `before-after` | state X transformed to state Y | STORY + NUMBER |
| `mechanism-reveal` | the "real reason" turn behind a visible symptom | SYMPTOM + ANALOGY + RULE |
| `mini-case-study` | single client transformation as proof | STORY + NUMBER + PROOF |
| `numeric-walkthrough` | staged small-input → big-number demo | NUMBER ×3-5 |
| `N-component-enumeration` | decompose an abstract into N named parts | CLAIM ×N + RULE |
| `objection-stack` | name + dismiss 2-3 likely pushbacks | OBJECTION ×N |
| `demo-then-principle` | show it working, then name why | PROOF + RULE |
| `stat-then-implication` | surprising data point → what it means | STAT + RULE |
| `story-with-extraction` | anecdote → the lesson pulled from it | STORY + RULE |
| `frame-name-drop` | name a concept/framework to make it sticky | CLAIM |
| `anti-list` | name what does NOT matter (authority consolidation) | CLAIM ×N |

New shapes require sign-off before entering the taxonomy (keeps the index searchable). Threshold: a shape must appear in 2+ source videos before it's added as a named shape.

---

## Slot types (what the user brings to fill a module)

| Slot | Content | Constraint |
|---|---|---|
| `NUMBER` | concrete numeric outcome | specific, not "thousands" |
| `STORY` | single client transformation | one arc, named subject |
| `CLAIM` | declarative assertion | ≤15 words |
| `ANALOGY` | outside-domain image | ≤15 words, single image |
| `RULE` | portable principle | ≤12 words |
| `SYMPTOM` | observable behaviour | concrete, not abstract |
| `STAT` | third-party data point | with source |
| `OBJECTION` | viewer pushback | in the viewer's words |
| `PROOF` | artefact / result | screenshot, dashboard, named number |

---

## Mix-and-match rules (composing a script)

1. **Match registers at the seam.** A module's `EXIT REGISTER` must equal or be adjacent to the next module's `ENTRY REGISTER`. High → low without a bridge breaks the script.
2. **Check the compatibility matrix.** Don't place two of the same shape back-to-back (two `numeric-walkthrough`s in a row drowns the viewer in numbers; two `N-component-enumeration`s kills the rhythm).
3. **Wire the loops.** If a module opens a loop it doesn't close (a `loop-debt`), the script must close it later or substitute a closer. If a module closes a loop it didn't open (a `loop-credit`), the script needs an upstream opener.
4. **Length-fit.** Sum of module length norms should land within ±15% of target runtime.
5. **Vary the shapes.** A "3 methods" or "5 steps" video is stronger when the steps use DIFFERENT shapes (step 1 = mechanism-reveal, step 2 = mini-case-study, step 3 = contrast-pair) than when all N use the same shape. Variety is the retention engine.
6. **Rotate case studies.** Track `last-used` per case (Foundr / Marianne / Tara / Jas / Gordon / Harlan / Danny / Ken). Any case used in the prior 3 scripts is deprioritised. Prevents over-rotation.

---

## How this plugs into the main workflow

- **Step 4 (build the outline):** instead of free-writing body bullets, pick the SHAPE for each body point from the taxonomy. The outline becomes: intro shape + body shape 1 + body shape 2 + ... + outro shape. This is the manual sequencing the skill requires — you're sequencing shapes, not delegating to Claude.
- **Step 7c (write each body point):** open the chosen module file, read its beat skeleton + slot specs, fill the slots with the user's content, write the body point in the user's voice hitting the beat functions. The module tells you the architecture; you write the sentences.

---

## IP / fair-use boundary (hard rules)

- Modules describe STRUCTURE (function, beat skeleton in structural verbs, length, slot specs, compatibility). These are method/idea, not protected expression.
- **Verbatim signature quotes:** capped at ≤12 words per module, only when the linguistic pattern itself is the lesson, default empty. Per-creator-folder total cap: 400 words across all files.
- **Never** stitch quoted beats into a runnable script. The bank produces SHAPES; the user writes the words.
- When composing a script from modules, the output sentences must be original — performing the same function as the source shape, never reproducing the source's phrasing.

---

## The bank (working library)

Lives at `template-bank/<creator>/`:
- `INDEX.md` — browse all modules by shape / section / case-fit, with last-used rotation tracker + quote-budget ledger
- `templates/t01...t10.md` — per-video architecture (arc, loop map, voice fingerprint, body section map)
- `modules/<id>.md` — the atomic cherry-pickable body-point modules
- `transcripts/` — source transcripts (reference only, never reproduced into modules)
- `_shapes/<shape>.md` — cross-creator rollup: every module of a given shape in one place, so you browse by what you need

First creator in the bank: **Kallaway** (10 videos, teaching-craft / personal-brand lane). 3 t01 modules fully built as the schema proof; remaining modules expandable on demand.
