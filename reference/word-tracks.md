# Word-Tracks — Kyle's exact correction prompts

These are the exact prompts the Educate.io product team uses to correct Claude when its output goes off the rails. Pull these out verbatim during the section-by-section review loop in Step 7.

The two workhorses are the **peeling-onion** correction (for punchy, disconnected, list-feeling output) and the **anti-AI-jargon** correction (for clichés and formulaic structures). They get used many times in a single scripting session.

---

## 1. The "two/three layers deeper" reset (universal Claude-laziness fix)

Use whenever Claude defaults to surface-level output, ignores nuance, or executes mindlessly without thinking through what you're trying to achieve.

> *"Pause. Think two, three layers deeper about what I'm actually trying to achieve here, not just the surface request. Then continue."*

This is the same instruction used at the end of the initial context prompt — it's the universal anti-laziness reset for Claude and gets used throughout the entire scripting session whenever output quality drops. Use it as often as needed.

---

## 2. The peeling-onion correction (for punchy, disconnected, list-feeling output)

Use whenever the output:
- Reads like a list pretending to be prose.
- Has too many short staccato sentences in a row.
- Each sentence stands alone instead of leading naturally to the next.
- Has the punchy "not X, not Y, but Z" rhythm AI defaults to.
- Feels like bullet points that have been smushed into paragraphs.

> *"Please rewrite this section so that it flows. Each sentence must flow one after the other. Each section flows one after the other. Build it in a way that's chronological and sequential — not punchy. Explain it in an explanatory manner that's easy to understand.*
>
> *When explaining concepts, peel back the layers of an onion to get to the point you're trying to make. You have to go through certain explanations first so that when you arrive at the point, it makes the most sense. Don't lead with the punchline — earn it through the explanation that came before it."*

The peeling-onion analogy is what reliably fixes this. Use it.

---

## 3. The anti-AI-jargon correction (for clichés and formulaic structures)

Use whenever you spot:
- Words from the banned list (`reference/banned-ai-language.md`).
- Bridges like "Here's the thing:", "Here's how:", "Pay attention to this:", "And here's why that's so important…"
- Numbered list framings disguised as prose ("First, X. Second, Y. Third, Z.").
- Meta-commentary like "Let me explain:" or "This is where it gets interesting:".
- Em-dash-heavy formal cadence.
- Corporate-speak ("strategic", "comprehensive", "leverage", "robust", "scalable").

> *"Please rewrite this. Stop using AI jargon, AI structures, AI phrases, formulaic copywriting structures, and copywriting clichés. No 'Here's the thing,' 'Here's how,' 'Pay attention to this,' 'And here's why,' 'The key is,' 'This is why,' or any colon-list openers. No 'unlock,' 'navigate,' 'leverage,' 'comprehensive,' 'strategic,' 'powerful,' 'game-changing,' or any of the buzzwords I gave you in the banned list. Make it sound like a real person speaking naturally — explanatory, conversational, plain. Each sentence earns its place by enabling the next."*

---

## 4. The teleprompter-natural correction

Use when the output is grammatically correct but doesn't sound like a real person speaking — too formal, walls of text, sentences too long for breath, or written-language-not-spoken-language.

> *"Rewrite this so it can be read off a teleprompter and sound natural. Line by line, not walls of text. Sentences need to be the length of a natural breath. Read each line out loud as you write — if it doesn't sound like something a real person would say, rewrite it. Match the cadence of [name]'s natural speaking style from the transcripts I gave you earlier."*

---

## 5. The narrative-weave correction

Use when a narrative was supposed to be instilled but is either missing or stated too explicitly.

> *"You're missing the [validation / democratization / attention / timing] narrative in this section, OR you've stated it too explicitly. Don't say it. Show it through specific examples and proof points woven naturally into the [Application / Framing / etc.] step. The viewer should walk away believing the conclusion themselves, without realizing they were led to it."*

---

## 6. The retention-loop correction

Use when the packaging section or a body point fails to open/close loops effectively.

> *"This section needs more retention engineering. There must always be something unresolved in the viewer's mind. At [specific point], open a loop — promise something you'll explain later. When you close that loop in [later section], immediately open another. Don't let the viewer feel like they have all the answers — give them just enough to keep them watching for the next thing."*

---

## 7. The chronological / non-jumping-around correction

Use when the body of a section moves through the material in the wrong order — e.g. revealing the conclusion before the setup, or jumping between concepts.

> *"Rewrite this in chronological / sequential order. Surface-level facts first, then deepen. Don't reveal the conclusion before the setup that earns it. Don't jump between concepts — finish one before starting the next. Each layer enables the next layer."*

---

## 8. The repetition-killer correction

Use when later sections repeat concepts already covered in earlier sections.

> *"You're repeating concepts I already covered in [section X]. Re-read the prior approved sections I pasted above. This section must pick up where the last one ended and add new ground — not re-explain what's already been said. If a concept needs reinforcement, reference it briefly and move on; don't re-teach it."*

---

## 9. The meet-AND-exceed expectations check (intro-specific)

Use after Claude writes the intro — read it and ask yourself the two questions, then correct if either fails.

If the intro doesn't meet expectations fast enough:

> *"The intro takes too long to confirm what the title promised. The viewer clicked because of [exact title] — they need to feel they're in the right video within the first few lines. Rewrite the opening to address what they came for immediately, then expand."*

If the intro doesn't exceed expectations:

> *"The intro meets the title's expectation but doesn't exceed it. Promise more than the title offered — something extra they'll get by staying. Add a line that makes them feel they're getting bonus value beyond what the title promised."*

---

## How to use these word-tracks during the session

After Claude produces a section:

1. Read it.
2. Run the eye-test: does anything feel AI-y, formulaic, punchy, or off-voice?
3. Check the relevant banned-language list (`banned-ai-language.md`).
4. If something needs fixing → pick the right word-track and paste it. **Be specific** about what needs fixing — quote the exact phrases that are wrong.
5. Approve the corrected version, then move to the next section.

By body point 3+, Claude has compounded enough learning that you'll need these word-tracks much less. That's the whole reason for keeping everything in one chat.
