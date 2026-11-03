# DataScienceProject_Team8

colab https://colab.research.google.com/drive/1IyhmGKqCidd6c7e2hvupGArPMATrFFDw?usp=sharing

# Greenhouse Gas Emissions and Rental Prices in UK Regions

A team data science project for the UCL Data Science Society Project Labs finance track, exploring the relationship between greenhouse gas emissions and private housing rental prices in regions of the UK.

## Research question

**How do private housing rental prices in regions of the UK affect greenhouse gas emissions?**

## Project overview

This project investigates whether UK regions with higher private housing rental prices tend to have higher or lower greenhouse gas emissions. We will combine regional rental and emissions data, explore geographic and temporal patterns, and assess the relationship using statistical analysis. The analysis will treat rental prices as the explanatory variable and greenhouse gas emissions as the outcome; causal effects cannot be established from this comparison alone.

Greenhouse gas emissions represent contributions to climate change. They do not directly measure local air quality or environmental damage overall.

## Datasets

We plan to combine two datasets covering a common period:

| Dataset | Required information | Source |
| --- | --- | --- |
| Greenhouse gas emissions | Annual emissions by region | Office for National Statistics |
| Private housing rents | Average monthly private rent by region and date | Office for National Statistics |

## Proposed analysis

1. Inspect the coverage, definitions and quality of both datasets.
2. Standardise regional identifiers, dates and units, and document missing values.
3. Visualise emissions and rents using maps, time-series charts and scatter plots.
4. Estimate the direction and strength of their association using correlation and regression.
5. Check whether results depend on outliers, the emissions measure or the years included.

We will distinguish comparisons between regions from changes within the same region over time. If sufficient annual data is available, an extension will account for persistent regional differences and UK-wide annual changes.

## Planned repository structure

```text
data/
  raw/             # Original data, where redistribution is permitted
  processed/       # Cleaned and joined data
notebooks/         # Cleaning, exploration and modelling notebooks
outputs/           # Figures and analysis tables
README.md
requirements.txt
```

This structure describes the intended organisation; analysis files and dependency instructions will be added as the project develops.

## Expected outputs

- A documented process for cleaning and joining the datasets
- Visualisations of regional emissions and rental patterns
- Statistical estimates with uncertainty and sensitivity checks
- A final presentation explaining the findings and their limitations

## Project status

Research question defined. Dataset selection and feasibility checks are the next steps. No findings have been established yet.
