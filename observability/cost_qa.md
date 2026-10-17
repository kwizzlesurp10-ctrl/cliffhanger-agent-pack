# Cost & QA Instrumentation

- Every turn logs tokens, estimated USD, tool calls
- QA gate runs rules + LLM-as-judge before staging
- Hard stop on budget_usd or max_turns
- Traces stored append-only for replay and regression

## Alerts
- Budget breach
- QA fail rate >15% over 5 drops
- Cache hit rate <90%
