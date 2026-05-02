# Banned AI Language — full sweep list

Every script gets scanned against this list before finalising. Any hit must be rewritten. The list is preserved verbatim from Kyle's documentation, expanded into clear groupings.

The point isn't that these words are *always* wrong — it's that they're the patterns AI defaults to, and they immediately signal AI-generated content to viewers. Cut them.

---

## How to use this list

Two-pass sweep before finalising:

**Pass 1 — Word-level grep.** Scan the full script (intro through outro) for every banned word and phrase. For each hit:
- Rewrite the sentence in plain natural language.
- If the word was load-bearing, find a specific concrete word that does the same job.

**Pass 2 — Pattern-level read.** Re-read the script for the formulaic structures and lazy bridges below — they're harder to grep but just as damaging.

If a script can't pass both passes, it's not done.

---

## 1. AI copywriting jargon and marketing buzzwords (banned outright)

```
comprehensive · identified · deep dive · mandatory · established · embarked
delved · invaluable · relentless · groundbreaking · endeavor · enlightening
insights · esteemed · shed light · underscores · crucial · delving · elevate
resonate · enhance · in the realm of · empower · unleash · unlock · intricate
tapestry · foster · systemic · inherent · treasure trove · testament · peril
landscape · pertinent · synergy · explore · folks · pivotal · adhere · amplify
cognizant · conceptualize · complexity · recognize · adapt · promote · critique
implications · complementary · perspectives · holistic · discern · multifaceted
nuanced · underpinnings · cultivate · integral · profound · facilitate · encompass
elucidate · unravel · paramount · characterized · significant · leverage
optimize · streamline · maximize · harness · revolutionize · transform · implement
execute · navigate · strategize · capitalize · pioneer · spearhead · orchestrate
curate · accelerate · propel · cutting-edge · state-of-the-art · innovative
dynamic · robust · seamless · scalable · agile · versatile · premier
sophisticated · meticulous · strategic · bespoke · tailored · personalized
customized · unparalleled · ecosystem · framework · methodology · paradigm
infrastructure · architecture · solution · platform · roadmap · blueprint
game-changer · best practices · thought leadership · stakeholders · deliverables
ROI · KPIs · metrics · furthermore · moreover · additionally · consequently
therefore · thus · hence · nevertheless · however · on the other hand
in conclusion · to summarize · moving forward · going forward · at the end of the day
results-driven · data-driven · customer-centric · solution-oriented · mission-critical
world-class · industry-leading · next-generation · future-proof · sustainable
actionable · in today's fast-paced world · stay ahead of the curve
take it to the next level · push the envelope · think outside the box
low-hanging fruit · circle back · touch base · move the needle
transformative · powerful · crushing it · quietly
```

**Words Kyle calls out by name as "stop watching immediately" triggers:**
- `strategic`
- `comprehensive`
- `quietly` (e.g. "quietly building", "quietly transforming")
- `powerful`
- `game-changing`
- `unlock`
- `navigate`
- `leverage` (as a verb — "leverage AI to…", "leverage the data")

---

## 2. Lazy bridges and formulaic transitions (banned outright)

These transitions announce that you're about to say something instead of just saying it. They're the AI tell.

```
Now, [topic]:
Here's how:
Let me explain:
So, [topic]:
[Number] things you need to know:
The [number] steps are:
First, [X]. Second, [Y]. Third, [Z].
Here's what you need to understand:
This is where it gets interesting:
Pay attention to this:
And here's why that's so important...
Here's the thing...
And that's exactly why...
Think about how...
This is why...
The key is...
This works because...
This creates...
The reason X matters is...
Notice that...
What you're doing is...
This distinction matters because...
Understanding X helps you...
```

Plus any sentence ending in a colon that introduces a list-like next chunk.

---

## 3. Formulaic copywriting structures (banned outright)

These aren't words — they're shapes Claude defaults to. Catch them at the pattern level.

- **Problem-Agitate-Solution** used mechanically (PAS isn't banned in spirit, just when it's done by-the-numbers without the natural cadence of someone actually thinking through the problem).
- **Numbered lists disguised as prose** — "First… Second… Third…" or "The three things you need to know are…"
- **"The three things you need to know" framing.**
- **Starting too many paragraphs with "The [noun]"** ("The reality is…", "The truth is…", "The key is…").
- **Constant "This is…" sentence starts.**
- **"For example:" followed by an italicised example in a box.**
- **Section-end summary statements** like "This is why X matters" / "This is exactly why this works."
- **Questions to the reader as engagement devices** ("Have you ever wondered…?", "What if I told you…?", "Sound familiar?").
- **Meta-commentary about what you're explaining** instead of just explaining it ("I'm about to break this down for you…", "What I want you to understand here is…").
- **The "not X, not Y, but Z" punchy triple** — AI's favourite rhythm. One use is fine; using it three times in a section is the giveaway.
- **Em-dash-heavy formal cadence** — long sentences chained with em-dashes feel written, not spoken. Use commas or full stops.

---

## 4. What to look for during the read-through

When reviewing the AI output, scan for:

| Symptom | What it looks like |
|---|---|
| **Disconnected flow** | Sentences that don't naturally lead into each other. Each one stands alone. |
| **Announcing instead of explaining** | "I'm about to tell you something" instead of just telling you. Meta-commentary. |
| **Staccato rhythm** | Too many short sentences in a row. Punchy. Listy. Like this. |
| **Corporate speak** | Formal language that doesn't sound like natural conversation. |
| **Generic claims** | "powerful" / "game-changing" / "transformative" without specific proof. |
| **Stitched-together feel** | The "not X, not Y, but Z" triple. The ratio-of-three pattern. The colon-list opener pattern. |

---

## 5. The brand-name carve-out

Brand names and proper nouns stay capitalized regardless of voice rules:
- Claude, ChatGPT, OpenAI, Anthropic, Google, YouTube, LinkedIn, etc.
- Specific people / companies / programmes named in the script.

Banned words still apply inside titles, hooks, and packaging unless they're proper nouns.

---

## 6. Quick-reference correction

When you find a hit, paste the anti-AI-jargon word-track from `word-tracks.md` (#3) into the chat with the specific phrases quoted:

> *"Rewrite [section] — you used [word] / [phrase] / [structure]. Stop using AI jargon, AI structures, AI phrases, formulaic copywriting structures, and copywriting clichés. Make it sound like a real person speaking naturally — explanatory, conversational, plain. Each sentence earns its place by enabling the next."*

---

## 7. The eye-test

If a viewer would cringe and click away when they hear a phrase — it's banned. Trust the cringe.
