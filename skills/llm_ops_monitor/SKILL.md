# Skill: LLM Ops Monitor

## Purpose
Track and report on the AI system's own usage patterns, cost efficiency, and reliability — keeping the orchestrator's operation profitable and stable as usage scales.

## When to use this skill
- User asks "how much are we spending," "check our AI usage," "is the system running efficiently," "cost report," or "usage summary."

## Process
1. If usage data is provided (request counts, token counts, costs), summarize: total requests, total cost, average cost per request, most-used skills.
2. Identify any anomalies: unusually expensive requests, repeated failed tool calls, skills rarely or never used.
3. Estimate monthly run-rate based on current usage pattern.
4. Compare current run-rate against budget (if budget is known) and flag if trending over/under.
5. Recommend optimizations if costs are trending high:
   - Reduce unnecessary context/memory window length
   - Cache frequently-requested skill instructions
   - Consolidate redundant skills
6. If no usage data is provided, explain what data is needed and how to export it (e.g., from provider dashboard or n8n execution logs).

## Output format
```
## Usage Summary
Total requests: ...
Total cost: $...
Avg cost/request: $...
Most used skill: ...
Least used skill: ...

## Run-rate estimate
Projected monthly cost: $...
Budget status: [Under/On track/Over]

## Recommendations
1. ...
2. ...
```

## Quality checklist
- [ ] All cost figures traced to actual provided data, not invented
- [ ] Run-rate projection clearly labeled as an estimate
- [ ] At least one concrete optimization recommended if trending over budget
