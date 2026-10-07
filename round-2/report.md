# round-2 — Investigate

**Team:** BB-029
**Queries used:** 76

## What we concluded

shipper_years has a strong, non-monotonic effect on the score. In our tested values, shipper_years = 32 produced the highest score of 0.9670.

## How we got there
We tested shipper_years values of 40, 32, and 30. The scores were 0.9609, 0.9670, and 0.9667 respectively, so 32 gave the highest observed score.


## What we ruled out

We ruled out the idea that simply decreasing shipper_years always increases the score, because reducing it from 32 to 30 decreased the score.

## What we are still unsure about

We are still unsure whether values close to 32 can produce a score higher than 0.9670, and whether other features interact with shipper_years.
