# Credit Risk Transition Modeling with Markov Chains and Monte Carlo Simulation

## Overview
This project models how borrowers transition between credit risk states over time using a Markov chain framework. Monte Carlo simulation is used to estimate default risk and evaluate how interventions affect long-run outcomes.

## Business Question
What is the probability that a borrower defaults over time, and how can improving early-stage recovery reduce overall risk?

## Why This Matters
Understanding how borrowers move through delinquency states allows lenders and policymakers to identify when risk is highest and where interventions are most effective. This model shows that early-stage improvements can compound over time, leading to meaningful reductions in long-run default exposure.

## Methodology
- Simulated borrower panel data
- Estimated transition probabilities between credit states
- Constructed a Markov transition matrix
- Simulated borrower paths using Monte Carlo methods
- Evaluated default risk over time
- Tested an intervention that improves recovery from delinquency

## Key Results
- Default risk accumulates rapidly in early periods
- Cumulative default probability reaches ~66% over 24 months
- Improving recovery transitions reduces default risk by ~1.3 percentage points over 24 months
- Effects are modest initially but compound over time

## Scenario Insight
Small improvements in early-stage recovery lead to persistent reductions in long-run default exposure.

## Example Output
![Cumulative Default](outputs/figures/cumulative_default_comparison.png)

## Limitations
- First-order Markov assumption
- Stationary transition probabilities
- Synthetic data
- No borrower-level heterogeneity

## Next Steps
- Segment transition matrices by borrower type
- Incorporate macroeconomic scenarios
- Compare with supervised learning models