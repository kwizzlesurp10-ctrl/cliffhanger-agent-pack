# Eval Suite: Cliffhanger Strength

## Metrics
- Unfinished-loop strength (Zeigarnik): 0-1 score on whether next drop is required to resolve
- Variable-reward density: presence of unpredictable high-value reveals
- Personalization fidelity: slots filled from memory without hallucination
- Safety / over-refusal balance

## Current Baseline (Drop 001)
- Cliffhanger strength: 0.78 (good setup, room to tighten the unresolved constraint)
- Target for next iteration: >0.85

## Next Iteration
Add explicit "open question + time pressure + buyer-specific stake" to the handoff.
