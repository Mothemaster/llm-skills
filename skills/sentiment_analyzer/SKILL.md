# Skill: Customer Sentiment Analyzer

## Purpose
Analyze customer reviews, support tickets, or social mentions to extract themes, emotional tone, and actionable insight — feeding real customer language into other skills (ads, product descriptions, support responses).

## When to use this skill
- User provides reviews, tickets, comments, or asks "what are customers saying about X" or "analyze sentiment."

## Process
1. Categorize each piece of feedback as Positive, Negative, or Neutral.
2. Extract recurring themes (e.g., "shipping delays," "great customer service," "confusing checkout").
3. Pull 3-5 direct customer quotes per theme — verbatim language is valuable for later copywriting use.
4. Calculate a rough sentiment ratio (% positive / neutral / negative) if enough data exists.
5. Identify the single most urgent negative theme (highest frequency + highest severity).
6. Identify the strongest positive theme (best candidate for marketing/testimonial use).
7. Recommend one action per major theme.

## Output format
```
## Sentiment Summary
Positive: X% | Neutral: X% | Negative: X%

## Top themes
1. [Theme] — mentioned X times
   Quote: "..."
   Recommendation: ...

## Most urgent issue
...

## Best marketing opportunity
...
```

## Quality checklist
- [ ] Themes backed by actual quotes, not just paraphrased
- [ ] Sentiment split quantified, not just described
- [ ] One clear "urgent" and one clear "opportunity" identified
- [ ] Recommendations are specific, not generic ("improve support")
