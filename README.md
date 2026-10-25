# NYC Motor Vehicle Collision Analysis

**Individual Data Analytics Project · Masaryk University · March 2024**

Exploratory and statistical analysis of motor vehicle collisions in New York City, examining temporal trends, geographic concentrations, vehicle categories, recorded contributing factors, and accident severity.

## Research questions

- When and where are reported collisions concentrated?
- Which vehicle categories and recorded contributing factors appear most frequently?
- Can regression methods help explore accident severity and casualties?

## Data source

The original report uses the **Motor Vehicle Collisions – Crashes** dataset published by [NYC Open Data](https://data.cityofnewyork.us/). Records include dates, times, locations, vehicles, casualties and contributing factors. The original analysis describes removing sparsely represented years and variables with extensive missingness; it does not establish exposure-adjusted accident rates.

## Methodology

The report describes an R-based workflow involving data cleaning, feature engineering, descriptive visualizations and regression models:

1. Explore and clean collision records.
2. Examine yearly, monthly, daily and hourly counts.
3. Compare boroughs, streets, vehicle types and recorded contributing factors.
4. Fit a **logistic regression** model for accident severity using an 80/20 split of a 10% sample.
5. Fit a **linear regression** model for casualty counts using a 75/25 split of selected records.

## Main observations

The report identifies differences across time periods, locations and vehicle categories, with higher recorded collision counts on weekdays and around busy travel periods. These are *descriptive counts*: without denominators such as vehicle miles travelled, they cannot be interpreted as relative collision risks.

## Interpretation and limitations

- Reporting thresholds, incomplete records, excluded observations and changing mobility patterns can affect comparisons.
- Model coefficients and classification performance must be interpreted alongside target definitions, class balance and validation.
- This observational study does **not** establish that the recorded factors caused accidents.
- Reproducibility is currently limited because the original R scripts, exact data extraction and model artifacts have not yet been added.

## Repository status

**Documentation-first release.** The research report and local analysis materials are being reviewed for a reproducible public release; do not treat this README as a complete executable workflow.

See [DATA_SOURCES.md](DATA_SOURCES.md) for sourcing and reproduction requirements.

## Related projects

- [Twitter Sentiment & Socioeconomic Analysis](https://github.com/swampyaepaing/twitter-sentiment-analysis)
- [Research portfolio](https://github.com/swampyaepaing)
