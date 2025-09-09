---

# IMDb Movies and TV Shows – Data Wrangling in R

The project demonstrates advanced data manipulation and wrangling techniques in R using the **tidyverse** framework, applied to IMDb/Netflix movie and TV show datasets.

---

[![Made with R](https://img.shields.io/badge/Made%20with-R-blue?style=flat&logo=r)](https://www.r-project.org/)
[![tidyverse](https://img.shields.io/badge/Package-tidyverse-green?style=flat&logo=r)](https://www.tidyverse.org/)
[![ggplot2](https://img.shields.io/badge/Visualization-ggplot2-orange?style=flat&logo=r)](https://ggplot2.tidyverse.org/)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0%201.0-lightgrey.svg)](LICENSE)

## Project Overview

The project involves:

* Cleaning, transforming, and analyzing two datasets:

  * **show\.csv** – Netflix movies and TV shows metadata
  * **MaturityType.csv** – maturity ratings descriptions
  * **Production.xlsx** – country-level production statistics with maturity type and rating data
* Performing advanced wrangling using `dplyr`, `tidyr`, and `ggplot2`.
* Answering structured questions by writing R code in an R Markdown (`.Rmd`) file.
* Generating insights, visualizations, and recommendations for content targeting and ranking.

---

## Key Tasks Implemented

### Part 1 – IMDb Shows and Movies

1. Loaded, cleaned, and renamed dataset columns.
2. Removed duplicates and standardized IMDb scores.
3. Filtered TV shows by country, year, and rating.
4. Extracted shows with specific keywords (e.g., *teen* and *high school*).
5. Identified top production countries for general audience shows.
6. Compared U.S. and Canadian movies (post-2010) using boxplots.
7. Designed a ranking system for children’s movies under 7 years old, implemented scoring, and recommended the top 5.

### Part 2 – Production and Continent Data

1. Cleaned and reshaped Excel data (pivoting, separating columns, fixing types).
2. Counted distinct countries and years after transformation.
3. Identified countries with average scores in a specified range.
4. Merged country–continent data and checked coverage.
5. Proposed a ranking system to help Netflix expand in Asia, ranked countries, and visualized results with bar charts.

---

## Techniques & Libraries

* **Data Wrangling**: `dplyr`, `tidyr`, `stringr`
* **Data Import**: `readr`, `readxl`
* **Visualization**: `ggplot2`
* **R Markdown**: For structured documentation and reproducible analysis

---

## How to Run

1. Clone this repository:

   ```bash
   git clone https://github.com/umair-statistics/imdb-data-wrangling-r.git
   cd imdb-data-wrangling-r
   ```
2. Open **Assignment.Rmd** in RStudio.
3. Make sure the following libraries are installed:

   ```r
   install.packages(c("tidyverse", "dplyr", "stringr", "readxl", "ggplot2"))
   ```
4. Knit the `.Rmd` file to HTML/PDF/Word to see the results.

⚠️ **Note:** Place the datasets (`show.csv`, `MaturityType.csv`, `Production.xlsx`) in the same directory as the `.Rmd` file before running.

---

## Files in Repository

* `Imdb_tidyverse.Rmd` – Main R Markdown solution file
* `show.csv` – Netflix movies and shows data
* `MaturityType.csv` – Maturity ratings metadata
* `Production.xlsx` – Production and continent-level data
* `README.md` – Project documentation (this file)

---

## Insights & Outcomes

* U.S. dominates general audience content production, but average IMDb scores vary.
* Canada and the U.S. show different IMDb score distributions in recent movies.
* Ranking criteria for children’s movies help parents make informed choices.
* Netflix can target Asian markets (e.g., Japan, Israel, Bangladesh, China) for expansion based on maturity-type performance.

---

## License

This project is for **educational purposes** (university assignment).
Feel free to reference but not to copy directly for submissions.

---
