# round-4 — Reconstruct

**Team:** BB-029
**Queries used:** 80 / 80

## What we concluded

We reconstructed the hidden decision behavior using the available data and observations from Rounds 1 and 2. Tree-based ensemble models gave the strongest results among the approaches tested. The reconstruction focuses on the relationship between the available shipment features and the final decision.

## How we got there
We combined the Round 1 and Round 2 datasets, giving 4,000 observations in total. The experiments tested classification approaches including Logistic Regression, K-Nearest Neighbors, Random Forest, and Extra Trees.
The strongest recorded experiment was an Extra Trees model, which achieved 89.17% accuracy on its internal test split. The final reconstruction used a Random Forest pipeline with preprocessing for numerical and categorical features.

Round 2 experiments also showed that `shipper_years` has a measurable effect on the model score. Reducing `shipper_years` from 40 to 32 improved the observed score, while reducing it further to 30 produced a slightly lower score.

## What we ruled out

Simple linear assumptions were not sufficient to explain the observed behavior. The experiments showed that tree-based models were better suited to capturing the nonlinear relationships between the shipment features and the decision.

We also did not treat the internal validation result as an official Round 4 score, because the current reconstruction notebook does not contain the separate official 80-point unseen validation set.

## What we are still unsure about
The exact hidden scoring and decision rules cannot be fully determined from the available Round 1 and Round 2 observations alone.

The reconstruction therefore represents an approximation of the hidden model rather than a claim that the original model has been exactly recovered.
## Colab Notebook

https://colab.research.google.com/drive/1d0JrbTzX6DWlArDunBGOivT3xY8oGpGf?usp=sharing


