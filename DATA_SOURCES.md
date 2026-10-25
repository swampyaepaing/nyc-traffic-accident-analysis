# Data sources and reproducibility

## Original dataset
**NYC Open Data: Motor Vehicle Collisions – Crashes.**

Official portal: https://data.cityofnewyork.us/

The March 2024 project report describes police-reported New York City crash data and a working period derived from records initially spanning 2012–2024. It documents exclusions for sparsely represented years and missing-value treatment. The precise dataset download date, snapshot, and inclusion criteria should be reconstructed from the original scripts before the figures are reproduced.

## Reproduction checklist

- [ ] Record the official dataset identifier and retrieval date.
- [ ] Recover and review the original R scripts.
- [ ] Document cleaning rules and all excluded observations.
- [ ] Identify the logistic regression target and predictors; check class balance.
- [ ] Report confusion matrix and appropriate predictive metrics.
- [ ] Document the linear regression outcome, sample-selection rules and residual diagnostics.
- [ ] Export source figures with captions and figure-generation scripts.

## Usage
Consult NYC Open Data for dataset licensing and attribution. Do not assume that reported incident counts measure collision *risk* without traffic-exposure denominators.
