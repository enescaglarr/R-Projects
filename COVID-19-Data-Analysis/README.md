# COVID-19 Data Analysis with R

## Overview
In this beginner-level R project, you'll step into the role of a data analyst exploring the global COVID-19 pandemic using real-world data. Leveraging **R** and the powerful **dplyr** library, this project manipulates, filters, and aggregates a comprehensive dataset containing information on COVID-19 cases, tests, and hospitalizations across different countries. 

By applying data wrangling techniques such as grouping and summarizing, the project identifies which countries have the highest rates of positive COVID-19 tests relative to their testing numbers. This hands-on project strengthens R programming skills and provides valuable experience in deriving actionable insights from real-world health data – a crucial skill in today's data-driven healthcare landscape.

---

## Tools and Technologies
- **R**
- **dplyr**
- **readr**
- **tibble**

---

## Prerequisites
To complete this project successfully, you should be comfortable with:
- Creating and working with **vectors**, **matrices**, and **lists** in R.
- Indexing data structures to extract elements for analysis.
- Applying functions to data structures to perform calculations.
- Manipulating and analyzing data using dataframes.

---

## Step-by-Step Instructions
1. **Load and Explore the Dataset**:
   - Use the `readr` package to load the `covid19.csv` file.
   - Quickly explore the dataset using functions like `glimpse()` and `head()`.

2. **Filter and Select Relevant Data**:
   - Filter rows for "All States" and remove irrelevant columns.
   - Create a focused dataframe with daily data on active cases, hospitalizations, and testing.

3. **Aggregate Data**:
   - Group data by `Country_Region` and calculate summary statistics for daily tests, positive cases, and hospitalizations.

4. **Identify Top Countries**:
   - Identify the top 10 countries by testing numbers.
   - Calculate the ratio of positive cases to tests and rank countries based on this ratio.

5. **Work with R Data Structures**:
   - Create and manipulate vectors, matrices, and lists to store key findings.
   - Combine results into a comprehensive list structure for easy interpretation.

---

## Expected Outcomes
Upon completing this project, you will have:
- **Analyzed** a real-world COVID-19 dataset using R and dplyr.
- **Manipulated data** to filter and aggregate meaningful insights.
- **Identified trends** from grouped data using summary statistics.
- **Created and worked with** R data structures like vectors, matrices, and lists.
- **Answered specific questions**, such as identifying countries with the highest positive test ratios.

---

## Key Code Highlights

### Load and Explore Data
```r
library(readr)
library(tibble)

# Load the dataset
covid_df <- read_csv("covid19.csv")

# Quick exploration
glimpse(covid_df)
