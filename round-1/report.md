# round-1 — Observe

**Team:** BB-028
**Queries used:** 76

## What we concluded

The experiments explored how different parameter configurations affected the system's overall score and decision.

The best recorded result from our experimentation was an overall score of **0.8559** with an **APPROVE** decision.

This result shows that the tested configuration was accepted by the system, but the experiments do not provide enough evidence to claim that any single parameter independently caused the observed result.

## How we got there

<!-- The experiments that mattered, in order. Why each one was worth a query. -->
We tested multiple parameter configurations and observed the resulting score and decision.

During the experimentation, we compared the outcomes of different configurations and used the observed score and decision to guide further testing.

The final recorded observation was:

- Overall score: **0.8559**
- Decision: **APPROVE**
- Total queries used: **76**

The corresponding experimental evidence is recorded in `round-1/findings.json`.

## What we ruled out

<!-- Hypotheses you rejected and what killed them. This section carries real marks. -->
We did not find sufficient evidence to conclusively attribute the final score to any single parameter.

Therefore, we ruled out making unsupported causal claims about individual features based only on the experiments performed.

## What we are still unsure about

<!-- Being honest here scores better than overclaiming. -->
We are still unsure about the independent effect of individual parameters on the overall score.

More controlled experiments would be required to determine whether changing a specific parameter consistently increases or decreases the score.

We also do not claim that the observed **0.8559** score represents the maximum possible score, since the parameter space was not exhaustively explored.
