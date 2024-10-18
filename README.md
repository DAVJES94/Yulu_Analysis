# Yulu Electric Cycles Demand Analysis

## Project Overview  
This project analyzes the factors influencing the demand for Yulu's shared electric cycles in the Indian market. The focus is on **Exploratory Data Analysis (EDA)** and **Hypothesis Testing** to identify trends, relationships, and significant predictors of demand. Key aspects of the study include testing the effects of working days, seasons, and weather on cycle rentals. 

---

## Table of Contents  
1. [Introduction](#introduction)  
2. [Objectives](#objectives)  
3. [Dataset Overview](#dataset-overview)  
4. [Analysis Steps](#analysis-steps)  
   - Exploratory Data Analysis  
   - Hypothesis Testing  
5. [Technologies Used](#technologies-used)  
6. [Installation](#installation)  
7. [How to Run](#how-to-run)  
8. [Results](#results)  
9. [Conclusion](#conclusion)  
10. [License](#license)  

---

## Introduction  
Yulu is India’s leading micro-mobility service provider, offering sustainable commuting solutions. This project aims to understand the factors that drive the demand for electric cycle rentals, enabling Yulu to optimize operations, pricing, and fleet management.  

---

## Objectives  
- **EDA**: Explore the structure and relationships within the dataset.  
- **Hypothesis Testing**: Validate assumptions regarding key factors affecting cycle rentals.  
  - Effect of working days on rentals.  
  - Difference in rentals across seasons.  
  - Influence of weather conditions.  
  - Relationship between season and weather.  

---

## Dataset Overview  
The dataset contains the following key features:  
- **Count**: The number of electric cycles rented.  
- **Working Day**: Whether it was a working day (1) or not (0).  
- **Weather**: Category representing different weather conditions.  
- **Season**: Season during which the rentals were recorded.  

The dependent variable is the **"Count"** of rentals, and independent variables include **Working Day**, **Weather**, and **Season**.  

---

## Analysis Steps  

### 1. Exploratory Data Analysis (EDA)  
- Import the dataset and examine its structure.  
- Check for missing values and data inconsistencies.  
- Analyze the distribution of variables using histograms and boxplots.  
- Explore relationships between dependent and independent variables using correlation and visualizations (scatter plots, heatmaps).  

### 2. Hypothesis Testing  
- **Objective**: Test key hypotheses to understand the impact of different factors on electric cycle rentals.  
- **Hypotheses Setup**:  
  - **Working Day Effect**:  
    - **H₀**: Working days have no effect on the number of cycles rented.  
    - **H₁**: Working days affect the number of cycles rented.  
  - **Seasonal Differences**:  
    - **H₀**: The number of cycles rented is the same across seasons.  
    - **H₁**: The number of cycles rented differs across seasons.  
  - **Weather Differences**:  
    - **H₀**: The number of cycles rented is the same across different weather conditions.  
    - **H₁**: The number of cycles rented varies across different weather conditions.  
  - **Weather-Season Dependency**:  
    - **H₀**: Weather is independent of season.  
    - **H₁**: Weather depends on season.  

### 3. Test Assumptions  
- **Normality Test**:  
  - Use **histograms**, **Q-Q plots**, or **Shapiro-Wilk test** to assess normality.  
- **Equal Variance Test**:  
  - Apply **Levene's test** to check for homogeneity of variances.  

> _Note: If assumptions fail, continue the analysis but validate results with visual interpretations and highlight exceptions in the report._  

### 4. Perform Hypothesis Tests  
- Set the **significance level (α)** (typically 0.05).  
- Perform appropriate statistical tests:  
  - **T-test**: For working day effect.  
  - **ANOVA**: For seasonal and weather-related differences.  
  - **Chi-Square Test**: To check dependency between weather and season.  
- **Calculate Test Statistics** and make decisions to accept or reject the null hypotheses.  
- **Draw inferences** from the analysis and provide actionable insights.  

---

## Technologies Used  
- **Python**  
  - Pandas, NumPy  
  - Matplotlib, Seaborn  
  - SciPy, Statsmodels  
  - Scikit-learn  

---

## Installation  
1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/yulu-demand-analysis.git
   cd yulu-demand-analysis
