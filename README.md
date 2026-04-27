# Arterial Stiffness and Cognitive Decline

## Project Overview
This dashboard explores the association between arterial stiffness, measured by 
pulse wave velocity (PWV), and cognitive decline in community-dwelling older adults. 
Interactive visualizations allow users to examine cross-sectional and longitudinal 
relationships across demographic subgroups.

## Live Dashboard
🔗 [View the interactive dashboard](https://zhangyy9-13.shinyapps.io/finalproject_4a/)

## Why This Matters
Arterial stiffness is a modifiable cardiovascular risk factor that may serve as an 
early marker for cognitive decline before clinical symptoms appear. Identifying this 
association can inform preventive strategies targeting vascular health to reduce the 
burden of dementia.

## Data Source
Data are from the Emory Healthy Brain Study (EHBS), a prospective community-based 
cohort study nested within the Emory Healthy Aging Study (EHAS), enrolling adults 
aged 50–75 years who were cognitively normal at baseline. The dataset is confidential 
and not publicly available; only the source code is provided in this repository.

## Dashboard Features
- **Baseline Association**: Scatter plot of PWV vs. MoCA score at enrollment, colored by PWV quartile
- **Survival Analysis**: Kaplan-Meier curves showing time to cognitive impairment by PWV quartile, with at-risk table
- **Demographic filters**: Filter both visualizations by sex, race/ethnicity, and education level
- **About the Data**: Dataset description and study population details

## Source Code
- `finalproject_4a.Rmd` — R Markdown file with Shiny app code for all interactive visualizations

## Dependencies
```r
library(haven)
library(dplyr)
library(ggplot2)
library(plotly)
library(survival)
library(broom)
library(tidyr)
library(shiny)
```# DATA555
Interactive dashboard exploring arterial stiffness and cognitive decline
