# Project 2: Air Quality Analysis (2018–2020)

This repository contains the analysis and code for Project 2 in the biostatistics programming course.  
The project cleans daily pollutant data (CO, Ozone, PM2.5), computes monthly summaries, and generates visualizations for 2018–2020.

## Project Overview
Air quality is an important environmental factor that influences population health, and pollutant concentrations often exhibit seasonal 
and year-to-year variability. This project analyzes daily air pollution measurements collected from the EPA monitoring station at the 
RDU Airport for the years 2018 through 2020. The datasets include three major pollutants: carbon monoxide (CO), fine particulate matter (PM2.5), 
and ozone (O3). The raw data contain several issues that require careful preprocessing, including duplicate entries, repeated measurements
for the same date, inconsistent formatting, and occasional negative concentration values caused by measurement error. To address these 
challenges, this project implements a custom data-cleaning function, process_air(), which standardizes variable names, converts date 
formats, removes duplicates, replaces negative values with zero, and averages repeated observations within each day. After cleaning, the
processed datasets are used to create monthly average pollutant summaries and generate exploratory visualizations. These plots highlight
seasonal trends, compare pollutant patterns across years, and provide interpretable summaries of air quality variation over time. The workflow 
demonstrates reproducible programming practices, clear data organization, and effective use of R Markdown for environmental data analysis.

Author: Yiyang Xue

Course: BIOSTAT 721 

Date: November 2025  

## Data Sources
- Air Quality Data: EPA monitoring station  
- Time Period: January 2018 – April 2020  
- Pollutants Measured:
  - Carbon Monoxide (CO) – Daily Max 8-hour concentration  
  - Fine Particulate Matter (PM2.5) – Daily mean concentration  
  - Ozone (O3) – Daily Max 8-hour concentration  

## Repository Contents
```
├── Xue_Yiyang_Project2.Rproj         # RStudio project file
├── Xue_Yiyang_Project2.Rmd           # Main R Markdown analysis
├── Xue_Yiyang_Project2.docx          # Final knitted report
├── AQ_2018.csv                       # 2018 air quality data
├── AQ_2019.csv                       # 2019 air quality data
├── AQ_2020.csv                       # 2020 air quality data
└── README.md                         # Project documentation
```

## Plots Included
- Figure 1: Monthly CO & Ozone concentrations with 95% CI  
- Figure 2: Monthly PM2.5 concentrations by year  

## Software Requirements
- R (version 4.x)
- tidyverse  
- lubridate  
- ggplot2
- readr

## How to Reproduce
1. Clone the repository  
2. Open the `.Rproj` file in RStudio  
3. Knit `Project2.Rmd`  


