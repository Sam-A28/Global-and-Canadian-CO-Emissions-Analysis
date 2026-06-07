# 🌎 Global & Canadian CO₂ Emissions Analysis

## Overview

This project explores greenhouse gas emissions at both a global and national scale using data visualization techniques in R. The analysis combines worldwide fossil CO₂ emission data with Canadian facility-level greenhouse gas reporting data to identify trends, compare countries, examine emission sources, and understand how emissions are distributed geographically and across industries.

The project was completed as part of an Information Visualization assignment and demonstrates data cleaning, transformation, exploratory data analysis (EDA), and visualization using the R ecosystem.

---

## Objectives

This analysis answers several key questions:

- Which countries produced the highest fossil CO₂ emissions in 2021?
- How have emissions changed over time for major emitting countries?
- Do countries with high total emissions also have high per-capita emissions?
- What emission sources contribute most to Canada's reported greenhouse gas emissions?
- How do emissions vary across Canadian industries?
- How are emissions distributed geographically around the world?
- How do emission sources differ between major emitting regions?

---

## Datasets

### Global Fossil CO₂ Emissions Dataset

The global dataset contains annual fossil carbon dioxide emissions for countries worldwide, including:

- Total emissions
- Coal emissions
- Oil emissions
- Natural gas emissions
- Cement production emissions
- Flaring emissions
- Per-capita emissions

**Time Period:** Multiple years (focused on 2002–2021)

---

### Canadian Greenhouse Gas Reporting Program (GHGRP)

The Canadian dataset contains facility-level greenhouse gas emissions reported by industrial facilities, including:

- Facility information
- Province/Territory
- Industry classification (NAICS)
- Emission source categories
- Total facility emissions
- Source-specific emissions

**Time Period:** 2022–2023 (focused on 2023)

---

## Technologies Used

- R
- R Markdown
- Tidyverse
- ggplot2
- sf
- ggthemes
- scales
- maps
- ggalluvial

---

## Project Structure

```text
├── CO2_Emissions_Worldwide.Rmd
├── GCB2022v27_MtCO2_flat.csv.zip
├── EmissionsSourcesGES-2022-2023.csv
├── README.md
└── Generated Visualizations
```

---

## Data Preparation

### Global Dataset

- Renamed columns for readability
- Converted data types
- Removed missing values
- Filtered 2021 data for comparative analysis
- Selected major countries for time-series visualization

### Canadian Dataset

- Selected relevant variables
- Standardized column names
- Cleaned text fields
- Created simplified emission source categories
- Aggregated emissions by source type
- Grouped industries for comparison

---

## Visualizations

### 1. Top 20 Countries by CO₂ Emissions

Displays the countries responsible for the highest fossil fuel CO₂ emissions in 2021.

**Key Insight:**  
A small number of countries contribute a significant proportion of global emissions, with China and the USA leading by a substantial margin.

---

### 2. Emission Trends Over Time

Tracks fossil CO₂ emissions from 2002–2021 for:

- Canada
- China
- United States
- India
- Russia
- Japan

**Key Insight:**  
Emission growth rates differ significantly between countries, highlighting varying industrialization and energy consumption patterns.

---

### 3. Total vs Per-Capita Emissions

Compares overall emissions against emissions per person.

**Key Insight:**  
Countries with the highest total emissions do not necessarily have the highest emissions per capita.

---

### 4. Canadian Emissions by Source

Breaks down facility-reported emissions into source categories such as:

- Stationary Fuel Combustion
- Industrial Processes
- Transportation
- Venting
- Flaring
- Waste

**Key Insight:**  
A small number of source categories account for the majority of reported emissions.

---

### 5. Emissions by Industry Group

Compares the distribution of emissions across major Canadian industries.

**Key Insight:**  
Some industries exhibit substantially higher emission variability and contain extreme outliers.

---

### 6. Global Emissions Choropleth Map

Visualizes worldwide fossil CO₂ emissions geographically.

**Key Insight:**  
Emissions are concentrated in heavily industrialized and highly populated regions.

---

## Skills Demonstrated

### Data Analysis

- Data cleaning
- Data transformation
- Exploratory Data Analysis (EDA)
- Statistical summarization

### Data Visualization

- Bar charts
- Line charts
- Scatterplots
- Pie charts
- Boxplots
- Choropleth maps

### Data Engineering

- Data wrangling with Tidyverse
- Dataset integration
- Feature creation
- Data aggregation

### Geographic Analysis

- Spatial data processing
- Map generation with SF
- Geographic trend visualization

---

## Key Findings

- Global CO₂ emissions are concentrated among a relatively small number of countries.
- Emission growth varies significantly across major economies.
- High national emissions do not always correspond to high per-capita emissions.
- Canadian emissions are dominated by a small set of industrial emission sources.
- Certain industries contribute disproportionately to overall greenhouse gas output.
- Geographic visualizations reveal strong regional emission patterns worldwide.

---

## Future Improvements

Potential enhancements include:

- Interactive dashboards using Shiny
- Time-series forecasting models
- Province-level Canadian emission analysis
- Machine learning models for emission prediction
- Additional environmental indicators such as methane and nitrous oxide emissions
- Animated visualizations showing changes over time

---

## Author

**Samir Ahmadi**

Information Visualization Project  
Ontario Tech University

---

## Sample Output

The project generates six visualizations:

- Top Emitting Countries
- Emissions Growth Trends
- Per-Capita vs Total Emissions
- Canadian Emission Sources
- Industry Emission Distribution
- Global Emissions Map

Together, these visualizations provide a comprehensive view of greenhouse gas emissions at both global and Canadian scales.
