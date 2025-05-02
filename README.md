## GROUP SEVEN PHASE 2 PROJECT
### Created by:

**Diana Mayalo**

**Lewis Mwaki**

**Margaret Kariuki**

**Antony Chege**

**Phanela Aluoch**

# Lights, Camera, Analytics: Exploring the Film Business
### *Merging Storytelling with Statistics to Understand Movie Success*

![pexels-brunomassao-2873486](https://github.com/user-attachments/assets/283b959b-1ebd-4bdb-9dab-19fec68190e1)

## **Introduction**
### **Statistical Data Analysis for Silverline Studios.**
This project delves into the intricate world of cinema, uncovering patterns and insights that can guide our future business in film.
We explore the factors that make a movie a box office hit. Using statistical techniques and visualizations, this project examines how genre, budget, runtime, and ratings work together to influence global film revenue.
This analysis will help our new studio make informed decisions about venturing into film, ensuring that we create films that resonate with audiences and achieve commercial success.

## Overview
This project analyzes movie industry data to uncover what drives box office success. By examining factors like genre, budget, runtime, and ratings, we use data science and statistics to guide smart decision-making for a new movie studio. The goal is to find what works and why.

---

## Business Understanding
The film industry is risky but rewarding. Production decisions like genre, budget, and target audience can make or break a movie's financial success. For us as Silverline Studios entering this competitive landscape, data-driven decisions must be made, not guesswork, to ensure an edge over competitors and overall commercial success.

This project is designed to provide data-driven answers to key business questions:

- Which genres consistently deliver the highest global revenue?

- Does runtime affect audience rating, total gross, and if so, by how much, and what can we learn from it?

- Does marketing and popularity directly correlate with total_gross, and if so, how can we exploit this to our advantage?

- Can we predict the total gross of a movie based on its genre? Use this information to target high grossing genres.

- How is our competition? Which studios are on an upward trend that we can confirm? What can we emulate from the continued success?

- Do indie and major studios, having different financial levels of muscle, have significantly different average_ratings? If so, how do we position ourselves to be competitive in the market?

- The goal of analyzing historical movie data and applying statistical techniques is to equip the studio with actionable insights that reduce risk, maximize profit potential, and guide smarter production investments.

---

## Business Objectives
1. Analyze the relationship between total gross revenue and other key factors, such as budget, genre, runtime, and user ratings, to determine which variables most significantly impact a movie’s overall financial performance.
2. Competition & Niche Analysis: How are studios fairing, what are they focusing on, and how are they performing, and what genres have been neglected but are worth exploring, based on multiple factors.
3. Analyze yearly trends in key movie performance metrics, such as global revenue, budget, genre popularity, and average ratings, to identify patterns and correlations that can inform strategic decisions over time. 

---

## Business Context
In a competitive and risky industry, this analysis provides a **data-backed foundation** for launching a successful film studio. It helps reduce uncertainty and improves decision-making for future productions.

---

## Project Synopsis
In the dynamic realm of filmmaking, understanding the elements that contribute to a movie's success is paramount. This analysis aims to dissect various facets of movies, ranging from genres and budgets to runtimes and ratings, to identify trends and correlations that can inform strategic decisions in movie production and distribution.

---

## Tools & Technologies

- **Programming Language**: Python  
- **Data Manipulation**: pandas, numpy  
- **Data Visualization**: matplotlib, seaborn  
- **Statistical Analysis**: scipy, statsmodels  
- **Development Environment**: Jupyter Notebook

---

## Data Understanding
This project combines information from two key datasets to explore factors influencing movie profitability:

### 1. `bom.movie_gross.csv`
Sourced from Box Office Mojo, this dataset provides **domestic and worldwide gross revenue** for a wide range of films.

Key columns:
- `title`: Movie title
- `studio`: Production studio
- `domestic_gross`: Revenue earned in the U.S.
- `worldwide_gross`: Total revenue across all regions
- `year`: Year of release

### 2. `im.csv`
This dataset enriches the analysis with **movie-specific features**.

Key columns:
- `title`: Movie title (used for merging datasets)
- `genre`: Primary genre classification
- `runtime`: Duration in minutes
- `budget`: Production budget (USD)
- `rating`: IMDb rating (audience sentiment proxy)
- `release_date`: Official release date

### Data Integration
The datasets were merged on the `title` column to align financial metrics with production and content features. Cleaning steps included:
- Removing rows with missing or zero values in `budget` or `revenue`
- Filtering out non-theatrical or ambiguous entries
- Converting monetary and time values to numeric types

This integrated dataset formed the foundation for all subsequent statistical analysis and modeling.

---

## Data Overview

The dataset encompasses a diverse collection of movies, featuring attributes such as:

- **Title**
- **Genre**
- **Budget**
- **Revenue**
- **Runtime**
- **Rating**

*Note: Data cleaning and preprocessing were applied to ensure accuracy and usability.*

---

## Loading Libraries and Data

We used essential Python libraries like **pandas**, **numpy**, **seaborn**, and **matplotlib** for data manipulation and visualization.  
The two datasets—`bom.movie_gross.csv` and `im.csv`—were loaded using `pandas`, cleaned, and merged on the movie title for unified analysis.

---

## Data Cleaning

To ensure reliable analysis, we performed several data cleaning steps:

- **Removed missing or zero values** in critical columns like `budget`, `revenue`, and `runtime`.
- **Filtered out non-theatrical releases** and irrelevant entries.
- **Converted data types** to numeric for analysis (e.g., budgets, gross earnings).
- **Merged datasets** on movie titles after trimming and formatting to ensure accurate joins.

These steps helped create a high-quality dataset suitable for statistical testing and modeling.

---

## Analytical Approach

1. **Data Cleaning**: Standardized formats, handled missing values, and removed irrelevant records.  
2. **Exploratory Data Analysis (EDA)**: Used visualizations to explore distributions and variable interactions.  
3. **Statistical Testing**:  
   - Correlation analysis  
   - Hypothesis testing (e.g., t-tests)  
   - Confidence intervals  
4. **Regression Modeling**: Evaluated predictors of revenue based on budget, ratings, and runtime.

---

## Visualizations
### Top-Grossing Studios
WB has consistently high been having a growth trajectory. Proven by trends, strength, and significance
This should advice our marketing branding teams to study their promotion strategy and see if they can replicate it, even if on a smaller scale.

![download](https://github.com/user-attachments/assets/6e8f6104-8312-486c-84b9-e87505d13ad8)

### Top-Rated Movie Lengths
There is a statistically significant but weak correlation between runtime category and ratings
Since shorter films are rated higher, the difference is not substantial enough to warrant a focus on runtime. Instead, we should focus on significant factors

![download](https://github.com/user-attachments/assets/8901b082-b878-425f-89c0-10b8e2d1c244)

### Predicting Genres’ Total Gross
We should ignore War and Sport movies, as their predicted revenue is lower than what we currently have
The Musical genre has a high predicted gross vs actual, and it is the number 1 genre to look into to maximize revenue

![download](https://github.com/user-attachments/assets/52c1712e-2228-4853-a102-7d70e4562671)

### Popularity of movies over time
Marketing in the industry has gone down over the years, as shown by the stark decline recently
This is a good opportunity for us to take advantage of this and market our movies to the audience

![download](https://github.com/user-attachments/assets/c747ea73-7f48-4fc7-981f-ae027e240b1f)

---

## Conclusions
- Silverline Studio should focus on really significant factors instead of lightly correlated factors like movie runtime length
- The general trajectory in revenue generated over the years is going up, indicating that this is a good industry to invest in.
- Spend more on marketing since it's proven that the industry has neglected marketing, but it significantly affects our revenue
- Invest in the genres that have a higher predicted gross than the actual gross
- Emulate the work ethic and other cultures of Warner Bros, as it's one of the few with a strong and proven upward trend

---

## Final Insights & Recommendations
- **Drivers of Revenue**
***Insight:*** Genre and popularity (vote count) most influence total gross.

***Recommendation:*** Focus on high-performing genre combos (e.g., Action-Comedy), optimize runtimes (~100–130 mins), and greenlight films with strong early interest.

- **Studio Strategy & Niche Opportunities**
***Insight:*** Major studios dominate key genres, but high-rated niche genres are often overlooked.

***Recommendation:*** Target underexplored genres with strong ratings to differentiate and capture untapped audiences.

- **Yearly Trends**
***Insight:*** Revenue and budgets are rising, but returns aren’t always scaling. Genre popularity shifts over time.

***Recommendation:*** Monitor trends to avoid genre fatigue, and time releases strategically for better market fit.

---

## Next Steps
**Feature Expansion:**
Add new variables like cast popularity, marketing spend, and release season to improve prediction models.

**Predictive Modeling:**
Use regression or machine learning to predict total gross based on key features (genre, budget, votes, etc.).

**Studio Benchmarking:**
Compare performance metrics across studios over time to identify strategic gaps and emerging competitors.

**Genre Forecasting:**
Analyze genre cycles and emerging trends using time series to anticipate future market shifts.

---
