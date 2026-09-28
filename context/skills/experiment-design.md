# Skill: Experiment design

A fill-in procedure for turning a product question into a measurable, honest
evaluation. Owned in spirit by the data role but usable by any agent.

## When to use

- Defining how to measure whether a change works.
- Before building instrumentation or launching a test.

## Procedure

1. State the **hypothesis**: if we do X, then behaviour Y changes because Z.
2. Define the **primary metric** that represents the intended outcome.
3. Define **secondary and guardrail metrics** (including comprehension,
   accessibility and customer-welfare guardrails).
4. Specify **segments** (users, market, device, journey stage).
5. Confirm **instrumentation**: are required events already captured reliably?
6. Choose the **method**: A/B test, holdout, before/after, or observational —
   proportionate to the decision and risk.
7. Note **threats to interpretation**: seasonality, selection effects, novelty.
8. Pre-register **decision rules** before seeing results where possible.

## Output format

- **Hypothesis:** …
- **Primary metric:** …
- **Secondary / guardrail metrics:** …
- **Segments:** …
- **Instrumentation status:** available / needs work
- **Method and duration:** …
- **Threats to interpretation:** …
- **Decision rule:** ship if …, hold if …
