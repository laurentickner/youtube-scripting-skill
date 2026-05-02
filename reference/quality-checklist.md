# Quality Control Checklist — final gate before finalising

Run every script through this gate before treating it as done. If any of the seven questions fails, rewrite. Then run the banned-language sweep (`banned-ai-language.md`). Only after both passes is the script finished.

---

## Pre-flight: Title formula check (BEFORE scripting starts, not after)

Before any section is drafted:

- [ ] Title is picked from `reference/title-formulas.md` — not invented
- [ ] Which formula? **B__ / N__** (cite the exact formula ID)
- [ ] Which exemplar outlier proves it? (cite from the file)
- [ ] Title is under 70 chars
- [ ] Title does not match any anti-formula in `title-formulas.md`
- [ ] Title contains: named tool ✅, dollar floor or named result ✅, ICP qualifier (if Channel 2) ✅
- [ ] Brand voice respected (lowercase except brand names + intentional CAPS)

**If any check fails → rewrite the title before drafting any sections.** Title shapes the whole script — fixing it after is a full rewrite.

---

## The 7 questions

### 1. Does this script create an irreversible identity transformation?
By the end, does the viewer hold a belief or self-perception they didn't have at the start? Have they crossed a line that's hard to uncross?
- ✅ Yes → "I'm someone who builds AI-leveraged businesses now, not someone who hires teams."
- ❌ No → "Cool, I learned 5 tactics about AI."

(Applies most strongly to **Main Channel** transformation-focused content. Less load-bearing on Business / Extended / evergreen videos — but every video should still leave the viewer different than they arrived.)

### 2. Would someone reading this off a teleprompter sound natural?
Read it out loud. Or imagine the on-camera person reading it cold off a teleprompter.
- ✅ Yes → It flows. Sentences are the length of a natural breath. No walls of text. Line by line. Sounds like the creator's actual cadence.
- ❌ No → Long compound sentences, em-dash chains, formal written-language constructions, words the creator wouldn't actually say.

For 10–15 min videos delivered in conversational format (e.g. car), the deliverable is **bullet points**, not teleprompter — but each bullet should still pass the "sound natural when spoken" test.

### 3. Does each sentence enable the next one (peeling onion)?
Read sentence by sentence. Does each one earn the right to the next by setting it up?
- ✅ Yes → A reader can't skip a sentence without losing the thread. Each layer enables the next layer.
- ❌ No → Sentences could be re-ordered without changing meaning. Punchy. Listy. Disconnected.

This is the primary AI failure mode. If it fails here, paste the peeling-onion word-track from `word-tracks.md` (#2).

### 4. Are we building knowledge chronologically, not jumping around?
Trace the flow of concepts.
- ✅ Yes → Surface facts → inference → application → big picture, in that order. Body Point N references concepts established in Body Point N-1, not concepts revealed later.
- ❌ No → Conclusion revealed before the setup that earns it. Body points reference each other out of sequence. Concept revealed in Body Point 3 used as if known in Body Point 1.

### 5. Have we removed all AI gimmick phrases and copywriting clichés?
Run the banned-language sweep (`banned-ai-language.md`).
- ✅ Yes → Zero hits across both passes (word-level grep AND pattern-level read).
- ❌ No → Even one hit means the script reads as AI-generated to the audience.

Specific high-frequency offenders to scan for first: *strategic, comprehensive, quietly, powerful, game-changing, unlock, navigate, leverage (verb), Here's the thing, Pay attention to this, This is why X matters.*

### 6. Is the transformation journey specific to THIS audience, not generic?
Re-read the intro and outro.
- ✅ Yes → The viewer feels "this was written for someone in my exact situation." Examples mirror their context. The democratization narrative is real, not theoretical.
- ❌ No → Generic "anyone can do this" framing. Examples are about people who don't resemble the viewer. The transformation feels theoretical.

### 7. Does the withheld information create leverage without feeling manipulative?
Trace the loops opened and closed across the script.
- ✅ Yes → There's always something unresolved keeping the viewer in. When loops close, a new one opens. Curiosity-driven, not bait-driven.
- ❌ No → All information dumped at once (no retention). OR loops opened that never close (feels manipulative). OR fake loops that promise more than they deliver.

---

## Then run the banned-language sweep

Per `banned-ai-language.md`:

**Pass 1 — Word-level grep.** Scan for every banned word. Rewrite each hit.

**Pass 2 — Pattern-level read.** Re-read for formulaic structures and lazy bridges (Here's the thing, colon-list openers, "First, X. Second, Y. Third, Z." patterns, etc.).

---

## Then trim length manually

Now decide if the script is too long. **Trim manually.** Remove sections that don't earn their place. Do NOT ask Claude to "shorten it."

---

## Then it's done

If it passed all 7 questions + banned-language sweep + manual trim → ship.

If it didn't → keep iterating in the same Claude chat using the word-tracks in `word-tracks.md`. Don't start a new chat. The compounding learning across the conversation is what makes the later iterations cleaner.

---

## Per-channel modifier

| Channel | Question priority |
|---|---|
| **Main** | All 7 questions matter. Identity transformation (#1), peeling onion (#3), and audience-specificity (#6) are the highest-leverage. |
| **Business** | #2 (teleprompter natural for sophisticated audience), #3 (peeling onion), #4 (chronological — your audience will spot non-sequiturs instantly), #5 (banned language is even worse to a sophisticated audience). |
| **Extended** | #2, #3, #4, #5 plus subtle reinforcement of unique-mechanism narratives (don't lose positioning even on goodwill content). |
