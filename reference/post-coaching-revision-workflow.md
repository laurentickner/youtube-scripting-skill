# Post-Coaching Revision Workflow

How to incorporate coaching feedback into a YouTube script that's **already been filmed** — without binning all the existing footage and refilming from scratch. Built from the 2026-05-24 Kyle Denyssen revision of Lauren's "$20k/m as an Online Coach" script. Use this whenever a coach reviews a filmed script and recommends structural changes.

> **The whole point of this doc:** if you treat every coaching note as "I must refilm everything from scratch," you'll burn days of production time. If you treat it as "ship as-filmed," you'll lose the structural lift the coach paid attention to. The middle path — Path B in this doc — keeps ~85% of existing footage usable while still addressing the coach's hard structural critiques.

---

## 1. The 3 paths after coaching feedback

### Path A — Full coach rewrite
Refilm intro + body 1 (or whatever the coach restructured) substantially. ~20-25 minutes of new spoken content. Maximum coach compliance. Cost: bins a lot of good existing footage.

**Use when:** the original script has fundamental issues (wrong frame, wrong hook structure, missing the audience's actual pain), the coach is explicit that everything needs to change, AND you have time + ability to refilm in matching conditions.

### Path B — Hard critiques only (default recommended)
Keep most existing footage; surgically add what the coach insisted on. ~5-10 minutes of new spoken content. Most of the existing cut survives. Coach's *insisted-on* fixes are baked in; coach's *polish* recommendations are intentionally skipped.

**Use when:** the existing content is fundamentally good, the coach's critiques are concentrated on specific structural fixes, AND/OR you can't easily refilm in matching conditions.

This is the default for most coaching revisions. The 2026-05-24 Kyle revision was Path B.

### Path C — Skip the revision
Ship the original as filmed. Skip the coach's feedback for this video.

**Use when:** the feedback is minor cosmetic, the video is already scheduled, AND the coach's critiques aren't structural. Risk: same issues will surface in the next coach review of the next script.

### Decision questions
- How much of my existing footage is still usable under the coach's recommended structure?
- Can I refilm new face-to-camera in matching conditions (same lighting, wardrobe, background)? If NO → defaults toward Path B with VO-only mode.
- How much time do I have before publication?
- Which of the coach's critiques are *hard-required* (he'll flag again next review) vs *polish* (nice-to-have)?

---

## 2. The Substance-Match Rule

The single most important rule for Path B. Where your existing filmed line covers the same *substance* as the coach's recommended line — even if the wording is slightly different — **use the existing take.** Don't force a new recording just because the wording isn't word-for-word identical.

### How to apply

For each new-content beat the coach recommends:

1. Read the coach's recommended text carefully.
2. Search your existing script (or filmed transcript) for any line that conveys the same substance.
3. If found, tag the beat as ✅ **EXISTING (substance-match)** — use that take. Note the slight wording difference for the editor.
4. If not found, tag as 🆕 **NEW VO** — record as voice-over.

### When the substance-match is borderline

If the coach's version adds 1-2 useful framings the existing footage lacks, consider:
- Option (a) — use the existing take and skip the addition (simplest)
- Option (b) — use the existing take + record a small NEW VO supplement that adds the missing framing (more work, more complete)

The 2026-05-24 Kyle revision used (b) for I-4 CREDIBILITY (existing decade-revenue line + new VO for "1,000+ clients" + "watched thousands of other coaches") and B-6 (existing rate-the-client + new VO supplement "the bar for who gets in has to be set by you, on purpose").

### What substance-match catches (real examples)

| Coach's line | Existing line | Verdict |
|---|---|---|
| *"Normally the client rates the coach, decides whether you were worth the money, leaves you a review at the end. With this framework, you rate the client instead."* | *"Normally the client rates the coach. Here, you rate the client."* | Substance-match. Existing covers the reversal mechanic cleanly. Coach's expansion (review-at-the-end / with-this-framework) is polish. ✅ Use existing. |
| *"I know how that sounds if your calendar is not full yet. The idea of declining anyone when you need the income feels insane."* | *"I know what that sounds like when your calendar is not full yet. Declining anyone feels insane when you need the income."* | Substance-match. Near-verbatim. ✅ Use existing. |

### What substance-match doesn't cover

If the coach's content is *fundamentally new* (a different framing, a different teaching, a different analogy), substance-match doesn't apply — record as NEW VO. Examples from the Kyle revision: the equation-analogy reverse-order callout, the two-kinds-of-client opener, the 5 APPLICATION beats, the criteria preludes ("criteria one"). None of these existed in any form in Lauren's original footage.

---

## 3. VO-Only Retrofit Mode (when you can't refilm face-to-camera)

Trigger conditions:
- Location change after filming
- Wardrobe / hair / makeup change
- Different lighting setup
- Different recording space
- Any condition where new face-to-camera would visually mismatch the original

### Hard rules

1. **All new content is voice-over only.** No new face-to-camera footage.
2. **Editor never cuts to your face during a new VO beat.** Visual mismatch will be obvious — wrong lighting, wrong background.
3. **Cut alternates** between original face-to-camera takes (for the parts you're keeping) and VO+B-roll moments (for new content).
4. **B-roll quality bar:** premium / WSJ-grade, not generic stock. See §6.
5. **Audio continuity:** EQ-match the new VO so it sounds like it's in the same room as the original. Don't ship if there's a noticeable audio shift.

### What this looks like in practice

The face → VO → face transitions become deliberate beats, not interruptions. The viewer should experience the alternation as "Lauren speaks → graphics teach a concept → Lauren returns" rather than "Lauren cuts away inexplicably."

### How to record VO that matches original face audio

- Use the same microphone if possible
- Record in the quietest room you have access to
- Speak in the same energy / pace / volume as your original takes (don't shift to a "voiceover voice")
- Record at the same time of day if possible (vocal cord state varies)
- Send the editor a brief audio sample from the original AND the new batch so they can EQ-match before cutting

---

## 4. The 3 deliverables (and what each is for)

A Path B revision produces 3 documents the editor needs:

### Deliverable 1 — Final Edit Script (canonical source-of-truth)
- The chronological flow of every beat
- Each beat tagged ✅ EXISTING / 🆕 NEW VO / cuts
- New VO content highlighted (yellow in Google Docs)
- B-roll cues inline per beat
- Recording checklist at the bottom (collapsed list of new beats for the operator's shoot)
- A header stating "if this conflicts with the editor brief, this script wins"

This is the document the editor cuts to. Template skeleton in §7.

### Deliverable 2 — Editor Brief (deeper reference)
- Full per-beat B-roll specifications (visual treatments, animations, on-screen text)
- Voice-over mode rules + quality bar
- Splice opportunities (optional fragments from original footage)
- Production notes
- Section explaining what changed and why

The editor reads this for context but defers to the Final Edit Script on what to cut.

### Deliverable 3 — Cover Note (Slack-ready intro)
- 1-page Slack/email-style intro
- Frames the project in 1 paragraph
- States the voice-over-only + B-roll requirements as the headline point
- Tells the editor which doc to read first (the brief)
- Lists files included

Lauren's editor-cover-note template at `_editor-cover-note.md` in the project folder.

---

## 5. Multi-Agent QA Before Shipping

Before sending the package to the editor, run 3 parallel QA agents:

### Agent 1: Coach Fidelity (structural)
- Verifies every hard structural critique the coach insisted on is addressed
- Verifies no new structural issues introduced by the retrofit
- Verifies the cut list is exhaustive (no orphan footage that should be binned)

### Agent 2: Coach Fidelity (content)
- Verifies the new VO content matches what the coach would want
- Verifies the substance-match reuses are appropriate (not losing meaningful content)
- Sweeps for banned words in the NEW VO scripts (per the operator's voice rules)

### Agent 3: Editor Usability
- Pretends to be the editor seeing the docs for the first time
- Walks through every beat trying to execute the cut
- Flags every place where instructions are ambiguous, missing, or where the editor would need to ask a question
- Checks the Google Docs paste-readability of the script (no markdown syntax that won't render)
- Verifies the source-of-truth between the 3 docs is unambiguous

Each agent saves its report to disk. Cross-check the 3 reports — items both Coach Fidelity agents flag are high-confidence issues. Items the Editor Usability agent flags are usability risks.

Synthesize into 3 buckets for the operator:
- 🔴 MUST-FIX — errors, typos, missing content, contradictions
- 🟡 DECIDE — judgment calls the operator needs to make
- 🟢 NICE-TO-HAVE — small enhancements that polish the result

Fix the MUST-FIXes silently. Surface the DECIDE bucket to the operator for decisions. Skip the NICE-TO-HAVE unless time permits.

### Agent prompt skeleton (for both Coach Fidelity passes)

```
You are auditing [operator's name]'s revision script against [coach's name]'s feedback.

== FILES TO READ ==
- The Final Edit Script
- The Editor Brief
- Any prior consolidated audit

== COACH'S VERBATIM FEEDBACK ==
[paste every coach comment verbatim — don't paraphrase]

== AUDIT CHECKLIST ==
[12-20 specific items mapped to the coach's critiques; each PASS / FAIL / CONCERN with quoted lines]

== DELIVERABLE ==
Save report to `/path/to/_qa-[agent-name].md`.
Reply with 4-line summary of findings.
```

Two Coach Fidelity passes (running in parallel, both reading the same coach feedback) catch ~95% of issues either alone would miss. The Editor Usability pass catches usability traps neither structural agent would notice.

---

## 6. B-Roll Quality Bar for VO Moments

When face-to-camera isn't available, the visual quality of the B-roll IS the production value. The bar:

### DO
- Clean motion graphics
- Type-driven visuals (large pull-quotes, key stats on screen)
- Real screenshots (Stripe receipts, DM threads with names obscured, dashboards)
- Animated equations
- Before/after splits
- Anonymised client logos, podcast covers, press mentions
- Subtle Ken Burns / parallax on stills
- Letter-by-letter reveals timed to audio
- Progressive visual scoreboards (e.g., 5-pointed star filling per criterion)

### DON'T
- Generic stock of "businesspeople shaking hands" / "person typing on laptop" / "diverse team in meeting room"
- Corny B-roll
- Cheap-looking animations
- Filler shots

### The mental bar
*"If you'd be embarrassed to show a frame to a private-banking client, rebuild it."*

Spell out per-beat B-roll specs in the Editor Brief. Don't tell the editor "design something appropriate" — that's how you get generic results. Tell them the exact visual treatment: what graphic appears, what text overlays where, what animation happens on which spoken phrase.

---

## 7. Templates

### 7a. Final Edit Script — skeleton

```
# Final Edit Script — [Section names] (vN)

**Canonical source-of-truth.** If this script and the editor brief disagree, this script wins.

> Reading conventions:
> - ✅ EXISTING = already filmed face-to-camera. Use the original take.
> - 🆕 NEW VO = operator records as voice-over. Highlight yellow. Editor uses B-roll throughout — never cuts to face during these.
> - 🎯 B-ROLL = visual treatment cue.
> - 🌟 STAR (or other progressive visual) = scoreboard fill timing.
> - Beat IDs cross-reference the Editor Brief.

## [SECTION NAME]

### [Beat-ID] Beat label
SOURCE: ✅ EXISTING — face to camera   (or 🆕 NEW VO — RECORD THIS — HIGHLIGHT YELLOW)

[The actual line, verbatim]

🎯 B-ROLL: [concrete visual treatment]

---

[…repeat for every beat in chronological order…]

## RECORDING CHECKLIST

Collapsed list of every 🆕 NEW VO beat with rough timing:
1. [Beat-ID] — [name] (~X sec)
2. […]

Total spoken time: ~X minutes. Plan a ~Y-minute session with safety takes.

## FILE REFERENCE

- `_editor-brief.md` — deeper reference
- `_editor-cover-note.md` — Slack-ready intro
```

### 7b. Editor Brief — skeleton

```
# Editor Brief — [video title]

## TL;DR for the editor
[1 paragraph framing: what changed, what to expect, default rule for ambiguity]

## 1.5 VOICE-OVER MODE — CRITICAL
[Hard rules: never face during VO, alternation pattern, audio continuity]
[B-roll quality bar with DOs and DON'Ts]

## 2. The NEW EDIT FLOW
[Every beat, chronological, with source tag + per-beat B-roll spec]

## 3. CUTS
[Original takes that should NOT appear anywhere]

## 4. SPLICE OPPORTUNITIES
[Optional fragments from original footage that can underlay new VO]

## 5. Production notes
[Visual cues carried from original brief + new specs]

## 6. File references

## 7. What to do if confused
[Escalate to operator, don't guess]
```

### 7c. Cover Note — skeleton

```
Hey [editor name],

Quick context. I filmed [video title], then got coaching feedback that restructured the [sections]. Everything from [unchanged section] onwards is unchanged — assemble from original footage in original order.

For the restructured sections I'm sending:
1. The ORIGINAL footage (you already have)
2. A second batch of VOICE-OVER ONLY recordings for the new beats

Critical:
- New beats are VO-only. Never cut to my face during them.
- You MUST design rich, intentional B-roll for every VO moment. No generic stock.
- The cut alternates between original face-to-camera and VO+B-roll moments.
- Audio continuity matters. EQ-match if needed.
- Substance-match rule: where my original take covers the substance of the new line, use the ORIGINAL.

Read `_editor-brief.md` cover-to-cover before you start. Numbered beat-by-beat guide.

Questions = flag before completing the cut, don't guess.

— [Operator]
```

### 7d. Recording checklist — skeleton

```
RECORDING SESSION — [date]

Setup:
- Same mic as original takes
- Quietest room available
- Match the energy/pace/volume of original takes
- Plan for 2 safety takes per beat

Order:
1. [Beat-ID] — [first line of beat]
2. […]
[…]

Total spoken time: ~X min
Estimated session length: ~Y min with safety takes
```

---

## 8. Common Failure Modes

- **Over-rewriting.** The instinct after a coach review is to refilm everything. Resist it. Substance-match aggressively. Only refilm where the coach's content is genuinely new.
- **Under-rewriting.** Skipping coach's hard structural critiques because "the existing footage is good." If the coach insisted on a fix, it goes in.
- **Ambiguous source-of-truth.** Operator produces 3 docs (script + brief + cover note) and they say slightly different things. Editor doesn't know which to trust. Always state explicitly: "this doc is canonical; here's the others."
- **Generic B-roll.** Editor ships stock footage of stock people because the operator told them "design something appropriate." Be specific in the brief — concrete visual treatments per beat.
- **Banned words slip into NEW VO.** Operator writes new content forgetting their own voice rules. Run a banned-word sweep on every new VO line before recording.
- **Forgetting the canonical source-of-truth header.** Add it to the top of the Final Edit Script every time. Saves an editor question later.
- **Skipping QA agents.** "I know the script is good." You don't. Run the 3 agents. The 30 minutes saves hours of editor back-and-forth.

---

## 9. The Operator's Pre-Ship Checklist

Before sending the package to the editor:

- [ ] Final Edit Script has the canonical-source-of-truth header
- [ ] Every beat tagged ✅ EXISTING or 🆕 NEW VO unambiguously
- [ ] Every 🆕 NEW VO beat is labelled in a way the operator can Find in Google Docs (e.g., "🆕 NEW VO — RECORD THIS — HIGHLIGHT YELLOW")
- [ ] Every beat has a B-roll cue
- [ ] Cut list in the Editor Brief is exhaustive
- [ ] All 3 QA agents have run; MUST-FIXes addressed; DECIDEs called by operator
- [ ] **Echo audit run** (§10) — framework name, element count, action verbs, outcome promises all under budget
- [ ] **Splice-opportunity audit run** (§11) — every new VO beat scanned for matching phrases in original footage; splice opportunities noted in the editor brief
- [ ] **Salvage audit run** — CUT-but-still-good footage (e.g., the carve-out) considered for face-time re-insertion
- [ ] Banned-word sweep on every new VO line (per `reference/banned-ai-language.md`)
- [ ] No markdown syntax in the script that will appear as literal characters in Google Docs
- [ ] Recording checklist at the bottom of the script
- [ ] "X minutes" placeholders in X2X / time-anchor beats filled in with the actual final runtime
- [ ] Cover note ready as a Slack/email paste
- [ ] Voice-continuity check planned (record a sample, A/B against original)

---

## 10. Echo Audit Before Recording

When you assemble beats from multiple sources (original face takes + new VO + substance-match reuses), the transitions between beats were never planned together. Repetition accrues silently. The viewer hears the same phrase twice in 30 seconds and the script feels amateur, even though each individual beat reads well in isolation.

Run an echo audit on the assembled script BEFORE you record the new VO. Two minutes of counting saves a re-record.

### How to run it

For each of the following high-frequency phrase families, count occurrences across the intro + body 1 SETUP (the densest part of any script):

- **Framework name** (e.g., "SCALE", "SCALE Equation") — should appear at most 3 times in the intro
- **Element count** (e.g., "five elements", "all five", "the five") — should appear at most 4 times in the intro
- **Action verbs you reach for as defaults** (e.g., "walk you through", "unpack", "show you") — should appear at most 1-2 times in the intro
- **Outcome promises** (e.g., "scale past that same number consistently", "$20k a month") — should appear at most 2 times in the intro

If a phrase exceeds the budget, identify which beat OWNS the meaning and CUT the restatements from the other beats. The first instance carries; subsequent instances erode.

### Common echo traps to look for

- **PREVIEW names the acronym → body 1 opener re-names it.** Fix: the body opener doesn't need to re-introduce the framework that was just named. Open the body with the angle, not the name.
- **X2X says "walk you through" → PREVIEW says "unpack every single one".** Same verb-class twice. Fix: pick the stronger one, drop the other.
- **BREAK BELIEF teases "five elements" → X2X restates "every one of those five elements" → PREVIEW restates "five elements".** Fix: BREAK BELIEF earns the number reveal; X2X can refer to "every one of them" (pronoun); PREVIEW can reference "the five" without re-saying "elements."
- **BREAK BELIEF close promises "scale past that number" → X2X echoes "scaling past that same number consistently".** Fix: X2X is a time-budget bridge. Drop the outcome restatement; the BREAK BELIEF close already landed it.

### The mental heuristic

> Each key concept gets named ONCE per ~60 seconds of intro. Pronouns and demonstratives ("them", "those five", "it", "this") replace re-naming.

If you find yourself writing "the SCALE Equation" three sentences in a row, you've lost confidence in your own framework. Cut.

### Real example (caught 2026-05-24 during the Kyle revision)

Across the assembled intro + B-1 opener, the term "five elements / five / all five" appeared 7 times and "SCALE / SCALE Equation" appeared 4 times in 90 seconds. Cuts that fixed it:
- I-2 BREAK BELIEF tightened close (dropped "and when those five elements are done right, they let you…" — replaced with "Done right, those five let you…")
- I-3 X2X dropped "so that just by following them, you can start scaling past that same number consistently"
- I-5 PREVIEW dropped "Each letter of the word SCALE stands for one of those five elements" (implicit) + dropped "Get all five working together, and the whole thing finally clicks into place" expansion
- B-1 dropped opening "It's called the SCALE Equation for a reason" (SCALE just named in I-5)

Net: ~40 fewer words across the intro. Same substance. Audibly more confident.

---

## 11. Splice-Opportunity Audit (face-time from existing footage)

In VO-Only Retrofit Mode (§3), new beats default to B-roll throughout — the editor can't cut to face during a VO beat because the new audio is from a different location. This is fine but leaves the cut visually heavy on B-roll.

The fix: scan the original filmed footage for phrases that ALSO appear in the new VO content. The editor can then splice short face-fragments from the original audio under the new VO B-roll, creating brief face-time moments inside otherwise VO-only beats. The operator's job is to FIND the matches and hand them to the editor.

### When to run it

After the Path B retrofit is mapped (existing vs new) and the new VO scripts are drafted. BEFORE finalising the editor brief.

### How to run it

For each new VO beat:

1. Pull up the new VO line(s).
2. Search the original filmed script (or transcript) for any phrase ≥3 words that appears in BOTH.
3. Match logic — accept:
   - Verbatim matches
   - Near-verbatim (1-2 word swaps, e.g., "you/I", "the/a")
   - Subject/tense swaps if the editor can crop tight on the matching fragment
4. Note in the editor brief as a SPLICE OPPORTUNITY under each beat: which fragment, from where in the original, what visual moment it could cover.

### Quality limits to spell out for the editor

- **At most 1-2 face-splice moments per VO beat.** More than that and the alternation feels frantic.
- **Tight cuts.** Splice on phrase boundaries, not mid-word. Audio joins should be invisible.
- **Audio continuity risk.** Original takes and new VO are from different sessions. Even after EQ-matching, subtle differences exist. Excessive splicing exposes the mismatch.
- **Lip-sync risk.** If the existing footage's lip movement doesn't match the new VO words exactly, the editor must cut to face AT the matching word and AWAY before the divergence. Tight-cut on the boundaries.

### Splice opportunities are OPTIONAL flexibility, not required

Default rule for the editor: use new VO + B-roll as the canonical treatment for every new beat. Splice in face fragments only where they add variety to a particularly long VO beat or where the matching phrase is unusually strong.

### Real example (mapped 2026-05-24 during the Kyle revision)

For Lauren's "$20k/m as an Online Coach" revision, the audit found these high-value splices for the editor:

| New VO beat | Matching fragment from original | Face-splice opportunity |
|---|---|---|
| I-5 PREVIEW: *"Get all five working together, and the whole thing finally clicks into place."* | Original PACKAGING: *"…how to **get all five working together**, in the right order…"* | Editor can cut to face on "get all five working together" mid-beat. |
| I-5 PREVIEW: *"…working way more hours for way less money."* | Original stakes line: *"…leave you **working way more hours for way less money**…"* | Editor cuts to face on the matching fragment — gives the stakes moment a face beat. |
| C1-3 APPLICATION: *"Even if the only person I solved it for was myself."* | Original C1 RULE: *"Even if **the only person you ever solved it for was yourself**."* | Editor cuts to face on the near-verbatim fragment (slight you/I subject swap, edit on the matching phrase). |
| C2-2 APPLICATION: *"Did they **reply to your messages** within a reasonable time?"* | Original C2-1: *"Watch whether they **reply to your messages**."* | Brief face moment on "reply to your messages". |

Without these splice maps, the editor defaults to B-roll across the entire I-5 PREVIEW and APPLICATION beats. With them, the cut alternates more naturally between face and B-roll, even in VO-only mode.

### Special case: salvaging cut content for face-time

Sometimes the substance-match audit and the Path B trims leave you with **cut-but-still-good** footage from the original. Examples from the Kyle revision: the carve-out *"I will not be teaching you how to coach. That is your zone of genius…"* was fully cut in Path B but is a high-quality face take that doesn't conflict with anything in the new structure.

If face-time is short, audit your CUT list for content that could be re-inserted as bonus face moments (not as required content). The carve-out can re-enter between I-4 CREDIBILITY and I-5 PREVIEW, for example, giving the viewer ~15 extra seconds of face after the credibility lands.

---

## 12. Source + exemplars

- 2026-05-24 Kyle Denyssen revision of the "$20k/m as an Online Coach" script. Logged in `coaching-feedback.md` 2026-05-24.
- Exemplar files (Path B implementation, in the project folder, not the skill):
  - `_final-edit-script.md` — full Path B script
  - `_editor-brief.md` — full Path B editor brief
  - `_editor-cover-note.md` — full Path B cover note
  - `_qa-kyle-agent-1.md` + `_qa-kyle-agent-2.md` + `_qa-editor-usability.md` — the 3 QA reports
  - `_kyle-changes-consolidated.md` — the before/after audit

When operating this workflow for the next script, start with the templates in §7 and adapt.
