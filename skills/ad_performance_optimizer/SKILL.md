# Skill: Ad Performance Optimizer

## Purpose
Analyze existing ad performance data and recommend specific, prioritized optimizations — closing the loop between ad creation and ad results.

## When to use this skill
- User provides ad metrics (CTR, CPC, ROAS, conversion rate) and asks "how do I improve this," "why is this underperforming," or "optimize my campaign."

## Process
1. Benchmark provided metrics against general industry norms (flag if CTR, CPC, or conversion rate are notably below typical ranges for the platform/industry, if known).
2. Diagnose likely cause by metric pattern:
   - Low CTR + normal conversion = creative/hook problem
   - High CTR + low conversion = landing page or offer mismatch problem
   - High CPC = targeting or bidding problem
   - Good early performance fading = ad fatigue, needs refresh
3. Recommend specific fixes tied to the diagnosed cause (not generic "improve your ad").
4. Prioritize recommendations by expected impact (highest first).
5. Suggest what to test next.

## Output format
```
## Performance diagnosis
Metric pattern observed: ...
Likely cause: ...

## Prioritized recommendations
1. [Highest impact fix] — why: ...
2. [Second fix] — why: ...
3. [Third fix] — why: ...

## Suggested next test
...
```

## Quality checklist
- [ ] Diagnosis is tied to specific metric patterns, not guesswork
- [ ] Recommendations ranked by expected impact
- [ ] At least one recommendation is immediately actionable (not a long-term strategy)
