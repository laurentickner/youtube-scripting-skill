# The Context Prompt — exact template

Paste this into a fresh Claude Sonnet 4.6 Extended chat at Step 5. Fill in every `{{ ... }}` block. **Do not paraphrase the closing instruction** — it's load-bearing.

---

```
You are an expert YouTube script writer and marketer.

Analyse all the information below regarding a new script I'm about to write.

═══════════════════════════════════════════
1. VIDEO DETAILS
═══════════════════════════════════════════

Title: {{exact video title}}

Channel: {{Main / Business / Extended}}
Channel viewer profile: {{2-4 lines describing who watches this channel — e.g.:
"Main Channel: broad appeal, mix of beginners and intermediates exploring online business; they want clarity, big-picture transformation, and they may not know our unique mechanism yet."
"Business Channel: sophisticated audience, established coaches / advisors / agency owners doing $100k+/mo, looking for high-leverage strategy."
"Extended Channel: smart beginners; they've found us already, watched the main channel, understand the unique mechanism, want more nuanced step-by-step depth."}}

Brief from {{name}}:
{{paste the brief verbatim — meeting transcript / Whispr-Flow notes / bullet points. Do not rephrase. If just a title was given, write: "Title only — no brief beyond what's in the title."}}

═══════════════════════════════════════════
2. CAMPAIGN CONTEXT
═══════════════════════════════════════════

Campaign objective:
{{What this video is engineered to achieve. Examples:
- "Warm up audience before the [event] lead-capture period — install Digital Products 2.0 as the new unique mechanism."
- "Drive opt-ins for the [event] during lead capture — viewer should click the description link and register."
- "Goodwill + nurture on Extended; reinforce that specialised AI is what makes Digital Products 2.0 accessible to beginners."
- "Evergreen authority piece for SEO — no CTA, build long-term trust."}}

Narratives to subtly instil:
{{For each narrative needed, name it and explain its psychological effect. Pick from these four (or your campaign's variant):

- ATTENTION narrative: makes the viewer feel like they're discovering something hidden in plain sight that most people are walking past. Positions them as "early adopters who see what others don't" rather than "late to the party."

- VALIDATION narrative: removes the risk of being wrong by showing credible, successful people are already doing this. Provides social proof that reduces decision anxiety. If respected people are doing it, pursuing this opportunity isn't foolish, it's what smart people do. Examples to weave in: {{specific named coaches / brands / experts already doing it}}.

- DEMOCRATIZATION narrative: removes the capability barrier by showing you don't need years of expertise, special skills, or unique advantages. Transformation: from "this works for other people but not for me" → to "this is specifically designed to work for someone in my exact situation." Makes the opportunity feel accessible to THEM.

- TIMING narrative: explains why NOW is the moment — not artificial scarcity, but genuine market conditions, technology shifts, or competitive dynamics that create a temporary window. Example: Bitcoin in 2012.

These narratives are NEVER explicitly stated. They are woven through the arguments, examples, and proof in the script.}}

Unique mechanism: {{e.g. "Digital Products 2.0 — Digital Products + AI"}}
Contributor (the enabler that makes the unique mechanism possible / accessible): {{e.g. "Specialised AI tools"}}

═══════════════════════════════════════════
3. SCRIPT STRUCTURE & OUTLINE
═══════════════════════════════════════════

Packaging (how the content is named/contained):
{{e.g. "5 rungs on a value ladder — DM Funnel → VSL Funnel → Application Funnel → Webinar Funnel → Challenge Funnel"
or "The Lazy Model Criteria (3 criteria framework) + 3-Step System"
or "8 Stages of Toxic Culture, central icon, numbered."
The packaging is the memorable container the audience walks away with.}}

Outline:

1. INTRODUCTION
   - {{bullet}}
   - {{bullet}}
   - {{bullet}}

2. PRESENT PACKAGING
   - {{bullet — what the framework is}}
   - {{bullet — why it matters}}
   - {{bullet — open the loops}}

3. BODY POINTS (chronological — keep this exact order)

   Body Point 1: {{name}}
   - {{bullet}}
   - {{bullet}}
   - {{bullet}}

   Body Point 2: {{name}}
   - {{bullet}}
   - {{bullet}}

   Body Point 3: {{name}}
   - {{bullet}}
   - {{bullet}}

   {{...add as many as needed}}

4. OUTRO
   - {{bullet — recap transformation}}
   - {{bullet — reassert unique mechanism}}
   - {{CTA bullets if applicable, otherwise: "no CTA — soft close"}}

═══════════════════════════════════════════

Analyse everything I've given you in-depth. Think two, three layers deeper about what I'm actually trying to achieve with this script, not just a surface-level understanding of the content. Once you've finished your analysis, wait for further instruction before continuing.
```

---

## Why the closing line is load-bearing

Claude defaults to executing tasks logically but mindlessly. The "two, three layers deeper / wait for further instruction" closer forces critical thinking and stops Claude from charging into output before it's understood the brief.

If during the chat Claude starts producing surface-level work, repeat the same instruction:

> *"Pause. Think two, three layers deeper about what I'm actually trying to achieve here, not just the surface request. Then continue."*

This is the universal Claude-laziness fix and gets used many times throughout a single scripting session.

---

## After the context prompt — what comes next

1. Wait for Claude's analysis. Read it.
2. If Claude has missed something material → correct it before moving on.
3. **Do NOT request the introduction yet.** First load the reference material in Step 6 (high-performing transcripts + creator natural-speech transcript + optional research).
4. Only then request Section 1: Introduction.
