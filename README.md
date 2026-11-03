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

| Dataset | Required information | Proposed source |
| --- | --- | --- |
| Greenhouse gas emissions | Annual emissions by region, with units and sector definitions | UK government regional greenhouse gas emissions statistics (coverage to be confirmed) |
| Private housing rents | Average monthly private rent by region and date | Office for National Statistics private rental price statistics |

The final dataset releases, download links, coverage and licences will be documented once selected. We will join records using consistent regional identifiers and year wherever possible. If rental observations are monthly, we will aggregate them to a consistent annual measure.

## Proposed analysis

1. Inspect the coverage, definitions and quality of both datasets.
2. Standardise regional identifiers, dates and units, and document missing values.
3. Visualise emissions and rents using maps, time-series charts and scatter plots.
4. Estimate the direction and strength of their association using correlation and regression.
5. Check whether results depend on outliers, the emissions measure or the years included.

We will distinguish comparisons between regions from changes within the same region over time. If sufficient annual data is available, an extension will account for persistent regional differences and UK-wide annual changes.

## Interpretation and limitations

- **Association does not establish causation.** Income, centrality, housing characteristics and economic activity may influence both emissions and rental prices.
- **Total emissions depend on regional population size and activity.** We will consider per-person emissions if suitable population data is available; this would require an additional data source.
- **Emissions sectors matter.** Industrial, transport and residential emissions may have different relationships with housing markets. We will state which sectors our measure includes.
- **Regional averages hide local differences.** Results will describe regional relationships and cannot establish the exposure or rent of an individual household.
- **Time coverage must be consistent.** We will use overlapping years and record any methodological changes in the source data.

## Planned tools

- Python and pandas for cleaning and analysis
- Matplotlib and seaborn for visualisation
- statsmodels for statistical modelling
- Jupyter notebooks or Google Colab for reproducible exploration
- GitHub for version control and collaboration

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
