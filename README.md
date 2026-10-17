# Cliffhanger Agent Pack

GitOps-friendly single-agent harness for generating uniquely addictive, sellable weekly serial digital content: multi-step prompt/agent packs with buyer-specific variable slots and cliffhanger handoffs.

Inspired by Anthropic's commerce-agents blueprint (skills over subagents, harness-enforced gates, async memory).

## Structure
- `config/agent-config.yaml`: Production config (model, budgets, gates)
- `src/harness.py`: Core agent loop with skills, memory, QA gate, packaging
- `evals/`: Evaluation suite for cliffhanger strength, quality, cost
- `drops/`: Generated packs (staged for approval)
- `observability/`: Cost/QA instrumentation notes

## First Drop
See `drops/drop-001-staged.md` (requires human approval before packaging/sale).

## Usage
```bash
# Local simulation
python src/harness.py --buyer demo --theme shadow-inventory
```

## Principles
- GitOps / IaC first
- Security, reliability, observability by default
- Hard budgets and approval gates
- Simple, maintainable, production-ready
