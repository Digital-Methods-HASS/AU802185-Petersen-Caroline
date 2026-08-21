# R Projects: Data Carpentry Coursework & Korea Gender Labor Market Analysis

This repository contains two R projects completed as part of coursework: a
data wrangling/visualization exercise using a Danish monarchs dataset, and
an independent analysis of gender-related labor market indicators in South
Korea compared to the OECD average.

## Repository Structure

```
.
├── monarchs/
│   ├── data/
│   │   └── Monarchs.csv
│   └── Monarchs.Rmd
│
├── korea_gender_labor_market/
│   ├── data/
│   │   ├── korea_gender_gap.csv
│   │   ├── korea_employment.csv
│   │   ├── korea_inactivity.csv
│   │   ├── gender_discrimination_perception.csv
│   │   └── korea_oecd_employment_by_age_2023.csv
│   ├── output/
│   │   └── combined_labor_indicators.png
│   └── korea_analysis.Rmd
│
└── README.md
```

## Project 1: Monarchs Assignment

A data wrangling and visualization exercise using a dataset of Danish
monarchs (name, birth year, death year, start and end of reign). Covers
reading semicolon-delimited data, calculating reign duration, handling
missing values, and visualizing reign duration over time using `ggplot2`.

## Project 2: Gender Labor Market Indicators — South Korea vs. OECD Average

An independent analysis comparing South Korea to the OECD average across
several gender-related labor market indicators:

- **Gender wage gap** (2004–2024)
- **Employment rate by gender** (1980–2025)
- **Labour market inactivity rate by gender** (1995–2025)
- **Employment rate by gender and age group** (2023)
- **Perceived discrimination by gender** (survey data, 2021)

Data sources: OECD Data Explorer (https://data-explorer.oecd.org/), and a
2021 survey by Hankook Research, commissioned by Hankook Ilbo. See the
metadata table in the report for full source details and access dates.

Data for most indicators was manually recorded from the OECD Data Explorer
interface into CSV files (semicolon-separated, comma decimals). The
age-group employment dataset was downloaded directly as an Excel export
and cleaned before use. See `data_visualization_writeup.md` for full
methodology notes.

## Software Requirements

- R (version 4.x recommended)
- R packages: `tidyverse` (`readr`, `dplyr`, `tidyr`, `ggplot2`), `patchwork`

Install dependencies with:
```r
install.packages(c("tidyverse", "patchwork"))
```

## License

- **Code**: Creative Commons Zero v1.0 Universal
- **Data**: OECD data reused under OECD's terms of use; survey data from
  Hankook Research/Hankook Ilbo is cited, not redistributed as original
  work.

## Contact

For questions, contact au802185@uni.au.dk.
