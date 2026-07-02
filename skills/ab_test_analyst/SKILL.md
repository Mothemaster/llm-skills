# Skill: A/B Test Analyst

## Purpose
Design A/B tests for content/campaigns and interpret results to recommend the winning variant and next test.

## When to use this skill
- User asks to "test two versions," "A/B test this," "which one performs better," or provides results data to interpret.

## Process

### If designing a test:
1. Identify the single variable to test (one variable per test — headline, CTA, image, price, subject line).
2. Write 2 (or more) clearly differentiated variants.
3. Define the success metric (CTR, conversion rate, open rate, etc.).
4. Recommend minimum sample size/duration for statistical relevance (rule of thumb: at least 100 conversions per variant before concluding).
5. State the hypothesis explicitly ("We believe X will outperform Y because...").

### If interpreting results:
1. Calculate the lift/difference between variants as a percentage.
2. Assess statistical confidence qualitatively (large sample + clear gap = high confidence; small sample + narrow gap = inconclusive).
3. Declare a winner only if the data supports it — otherwise recommend continuing the test or trying a bigger variable change.
4. Recommend the next test to run based on what was learned.

## Output format
```
## Test hypothesis
...

## Variant A
...

## Variant B
...

## Success metric: ...
## Recommended sample size/duration: ...

--- (when results provided) ---

## Results
Variant A: X% | Variant B: X%
Lift: +X%
Confidence: [High/Medium/Low/Inconclusive]
Winner: ...
Next test to run: ...
```

## Quality checklist
- [ ] Only one variable changed between variants
- [ ] Clear success metric defined before test starts
- [ ] Confidence level stated honestly, not overstated
- [ ] A concrete next step always provided
