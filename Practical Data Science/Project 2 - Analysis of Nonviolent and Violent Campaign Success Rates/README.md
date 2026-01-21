# Ioannis Michalopoulos - MSc Data Science, Athens University Of Economics And Business Department of Informatics
# Analysis of Nonviolent and Violent Campaign Success Rates

## Project Description
This project explores the historical trends and determinants of success for political campaigns globally from 1940 to 2014. Using data from the NAVCO (Nonviolent and Violent Campaigns and Outcomes) project and the Polity V dataset, the analysis examines whether nonviolent resistance is more effective than violent insurgency in achieving political objectives.

The study includes longitudinal visualizations of campaign frequencies and a logistic regression model to identify the statistical significance of nonviolence on campaign outcomes while controlling for popular participation and regime type.

## Technologies Used
* Python 3.11
* Pandas: Data manipulation and analysis
* NumPy: Numerical computing
* Matplotlib & Seaborn: Data visualization
* Plotnine: Implementation of a grammar of graphics in Python
* Statsmodels: Statistical modeling and logistic regression
* Scipy: Scientific computing

## Dataset Information
The analysis utilizes two primary data sources:
1. NAVCO 1.2 Dataset: Contains records of 389 strategic-level transitions, categorized by method (violent or nonviolent), location, participation levels, and outcome.
2. Polity V Dataset: Provides longitudinal data on regime characteristics and transitions to account for the political environment of the target governments.

## Project Pipeline

### 1. Data Cleaning and Preprocessing
* Importing raw Excel data.
* Transforming time-series data into decadal intervals for trend analysis.
* Calculating success percentages for different campaign categories.

### 2. Exploratory Data Analysis (EDA)
* Visualization of the frequency of violent vs. nonviolent campaigns per decade since 1940.
* Comparative analysis of success rates specifically for nonviolent movements over time.

### 3. Statistical Analysis
* Implementation of a Logistic Regression model.
* Independent Variables: Campaign method (Nonviolent/Violent), Participation level (log-transformed), Population (log-transformed), and Regime Type (Polity score).
* Dependent Variable: Campaign Success (Binary).

## Key Results
The regression analysis shows that the variable representing nonviolent campaigns (NONVIOL) yields a p-value of 0.001. This indicates that nonviolent methods have a statistically significant positive impact on the likelihood of a campaign's success, even when adjusting for the level of popular participation and the democratic/autocratic nature of the target regime.

## How to Use
1. Ensure you have the required datasets (`NAVCO 1.2 Updated.xlsx` and `p5v2018.xls`) in the same directory as the notebook.
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn plotnine statsmodels scipy
3. Open and run the notebook file in a Jupyter environment.   