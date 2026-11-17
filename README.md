# DataScienceProject_Team8

colab https://colab.research.google.com/drive/1IyhmGKqCidd6c7e2hvupGArPMATrFFDw?usp=sharing

# Dwelling Supply, Population and Private Rent Growth in England

A team data science project for the UCL Data Science Society Project Labs finance track.

## Research question

**How are changes in dwelling supply and population associated with changes in private rental prices across English local authorities?**

## Project overview

This project investigates 
## Datasets

We plan to combine three datasets at local authority level over a common period.

| Dataset | Required information | Source |
| --- | --- | --- |
| Dwelling supply | Dwelling stock counts by local authority and year | Government dwelling stock estimates |
| Population | Annual population estimates by local authority | ONS mid-year population estimates |
| Private rental prices | Average monthly private rent by local authority and date | Office for National Statistics (ONS) private rental price statistics |

## Regression model

We will fit a multiple linear regression with one observation per local authority over the same analysis period.

$$
\mathrm{RentGrowth}_i = \beta_0 + \beta_1\mathrm{SupplyGrowth}_i + \beta_2\mathrm{PopulationGrowth}_i + \varepsilon_i
$$

| Variable | Role | Definition |
| --- | --- | --- |
| Rental price growth | Dependent variable (Y) | Percentage change in average private rent |
| Dwelling supply growth | Independent variable (X₁) | Percentage change in dwelling stock |
| Population growth | Independent variable (X₂) | Percentage change in resident population |

Here, $i$ indexes local authorities, $\beta_0$ is the intercept, and $\varepsilon_i$ is the error term. $\beta_1$ estimates the difference in rental price growth associated with a one percentage point increase in dwelling supply growth, holding population growth constant. $\beta_2$ estimates the corresponding association with population growth, holding dwelling supply growth constant.

## Proposed analysis

1. Check the coverage, definitions and geographic boundaries of the source data.
2. Join the data and calculate percentage changes over the same period for all three measures.
3. Visualise the measures and their relationships with maps and scatter plots.
4. Fit the regression and report the coefficients with confidence intervals.
5. Check how sensitive the estimates are to influential local authorities and the analysis period, where coverage permits.

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
