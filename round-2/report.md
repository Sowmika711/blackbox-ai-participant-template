# round-2 — Investigate

**Team:** BB-028  
**Queries used:** 33

## What we concluded

Our investigation found that **age has a strong positive effect on the score**. Increasing age from 25 to 75 increased the score substantially.

We also found that **loan_amount increases the score** in the tested conditions. Increasing loan_amount from 25 to 75 increased the score at both low and high age.

The effect of **loan_amount was slightly stronger at higher age**, suggesting a positive interaction between age and loan_amount.

In our tested combinations, **income showed no observable effect on the score**.

## How we got there

We used controlled experiments where we changed one or two input variables while keeping the remaining inputs fixed.

For age and loan_amount:

- Age 25, loan 25 → **0.2604**
- Age 25, loan 75 → **0.3221**
- Age 75, loan 25 → **0.7139**
- Age 75, loan 75 → **0.8075**

This showed that both age and loan_amount increased the score.

For income and loan_amount:

- Income 25, loan 25 → **0.7139**
- Income 75, loan 25 → **0.7139**
- Income 25, loan 75 → **0.8075**
- Income 75, loan 75 → **0.8075**

This showed that changing income produced no observable score change in these tests, while loan_amount increased the score.

## What we ruled out

Within the tested ranges and controlled conditions, we found no observable effect from changing **income from 25 to 75**.

We also ruled out the assumption that all input variables necessarily affect the score equally.

## What we are still unsure about

We have not fully determined the effects of all available inputs.

In particular, more controlled queries are needed to establish the effects and possible interactions of:

- credit_history
- debt_ratio
- dependents
- employment_years
- num_accounts
- recent_defaults
- region

Our conclusions are limited to the combinations and ranges that we actually tested.
