# Round 1 — Observe

## Investigation

We tested different input configurations on the BLACKBOX AI system and recorded the resulting scores.

## Observations

The initial baseline configuration produced a score of 0.9581 with an APPROVE decision.

We then tested configurations with changes to multiple input features. These produced lower scores including 0.1005, 0.1263, and 0.1717.

A later configuration close to the baseline produced a score of 0.9581.

## Conclusion

The experiments show that the combination of input features affects the system score. The baseline configuration produced the highest score observed during our experiments.

However, some experiments changed multiple features at the same time, so we cannot confidently determine the individual effect of every feature yet.

## Next Steps

For future experiments, we would change one feature at a time while keeping the other inputs fixed. This would help identify which features have the strongest effect on the score.
