# Airbnb Los Angeles Price Analysis

**Tools:** R | ggplot2 | dplyr | tidyverse  
**Course:** MIS 431 – Data Mining for Business Applications  
**Institution:** George Mason University – Costello College of Business  
**Dataset:** 45,533 Airbnb listings in Los Angeles

---

## Overview

This project analyzes what drives Airbnb rental prices in Los Angeles —
one of the most active short-term rental markets in the United States.
Using R and ggplot2, the analysis explores how property type, room type,
and bedroom count influence listing prices across 45,000+ listings.

The goal is to help property owners and real estate analysts understand
pricing patterns and make data-informed decisions about listing strategy.

---

## Business Questions

1. How does **property type** affect Airbnb pricing?
2. How does **room type** influence rental rates?
3. How does **bedroom count** impact price distribution?
4. Which listings command the **highest prices** and why?

---

## Methods

| Step | Tool |
|---|---|
| Data loading & cleaning | `readr`, `dplyr` |
| Price normalization (remove $, filter outliers) | `dplyr::mutate`, `gsub` |
| Grouping & summarization | `dplyr::group_by`, `summarise` |
| Visualization | `ggplot2` |

**Visualizations produced:**
- Box plot — price distribution across top 10 property types
- Bar chart — average price by room type
- Histogram — price distribution by bedroom group (1–2, 3–4, 5+)

---

## Key Findings

**Property Type**
Entire homes and unique properties (guesthouses, villas) command
significantly higher prices than standard apartment listings.

**Room Type**
Entire home/apartment listings average considerably higher rates
than private or shared rooms — guests pay a premium for privacy.

**Bedroom Count**
Price increases with bedroom count, but begins to plateau at 5+
bedrooms, suggesting a ceiling on what guests will pay regardless
of size.

---

## How to Run

1. Clone this repository
2. Place `listings.csv` in the project root  
   *(Dataset available at [Inside Airbnb](http://insideairbnb.com)
   or [Kaggle](https://www.kaggle.com))*
3. Open `AirBnb_Midterm_Project_Draft.Rmd` in RStudio
4. Click **Knit** to render the full report with all visualizations

**Required R packages:**
```r
install.packages(c("tidyverse", "ggplot2", "dplyr", "readr"))
```

---

## Skills Demonstrated

- Exploratory data analysis (EDA) on a large real-world dataset
- Data cleaning and transformation in R
- Multi-variable visualization with ggplot2
- Business-driven insight generation from raw data
- R Markdown for reproducible reporting

---

## Author

**Ruszel Lee Velasco**  
B.S. Business – Management Information Systems  
George Mason University, 2025
