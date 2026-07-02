# Skill: Brand Voice Guardian

## Purpose
Enforce consistent brand voice, tone, and terminology across all content produced by any other skill — the quality-control layer for the whole system.

## When to use this skill
- User asks to "check this for brand voice," "make this sound like us," "review consistency," or provides a brand voice guide to apply.
- Should also be invoked as a review pass after other content-generation skills when brand consistency matters.

## Process
1. If a brand voice guide is provided, extract: tone descriptors (e.g., playful, authoritative, warm), banned words/phrases, preferred terminology, sentence length/complexity preference.
2. If no guide is provided, ask the user for 2-3 example pieces of content that represent their ideal voice, and infer tone patterns from them.
3. Review the target content against these criteria:
   - Tone match (does it sound too formal/casual relative to the guide?)
   - Terminology consistency (correct product names, no banned words)
   - Sentence rhythm (short punchy vs. long flowing, matching brand style)
   - Consistency of person/POV (we vs. I, formal "you" vs. casual "you")
4. Flag specific lines that break voice, with a suggested rewrite for each.
5. Provide a corrected final version.

## Output format
```
## Voice check results

### Issues found
1. Line: "..." — Issue: [too formal/off-brand term/etc.] — Suggested: "..."
2. ...

## Corrected version
[Full rewritten content]
```

## Quality checklist
- [ ] Every flagged issue includes a specific suggested fix
- [ ] Final corrected version provided in full, not just notes
- [ ] No new factual claims introduced during voice correction
