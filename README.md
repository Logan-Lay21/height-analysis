# Historical Height Analysis Across Five Datasets

A cross-century analysis of male height distributions using five datasets spanning Bavarian military conscripts, German prison records, SE German soldiers, BLS survey respondents, and the Wisconsin NSFH. Built as a DS350 project at BYU-Idaho.

---

## Overview

The project asks a simple question: do humans appear to have gotten taller over time when you look at individual-level data across five historical sources? Getting there required harmonizing five datasets with very different structures, units, and collection methods into a single comparable table — then being honest about what the visualization can and can't tell us.

## Key Findings

A subtle upward drift in median height is visible moving from the German military datasets (clustered around 67–68 inches) toward the American survey datasets (nudging 69–70 inches). However, the datasets are not a controlled comparison — three draw from German military and prison populations with minimum height requirements that cut off the lower tail of the true distribution, and then the comparison jumps to American survey respondents entirely. The trend appears real, but selection bias and population differences across these five studies make it difficult to isolate time as the cause.

## Data Sources

| Dataset | Population | Birth Years |
|---|---|---|
| Bavarian Conscripts | German military | 1800s |
| Bavarian Prison | German prison records | 1800s |
| SE German Soldiers | Military records | 1800s |
| BLS Heights | US survey (male) | ~1950 |
| Wisconsin NSFH | US survey | 1900s |

## Tools Used

| Tool | Purpose |
|---|---|
| R | Core language |
| tidyverse / dplyr | Data wrangling |
| haven | Reading Stata (.dta) and SPSS (.sav) files |
| foreign | Reading DBF files |
| ggplot2 | Violin + boxplot visualization |
| Quarto | Report rendering |

## How to Run

1. Clone the repo
2. Open the `.qmd` file in RStudio or Positron
3. Render with Quarto — data is pulled from public URLs at render time, no local data files needed
