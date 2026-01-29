# Global Internet Usage and GDP Analysis (2001–2024)
This project explores the historical trends and economic correlations between internet penetration and Gross Domestic Product (GDP). 
Using a dataset covering multiple countries over two decades, the analysis categorizes nations into "Developed" and "Developing" groups to observe differing growth trajectories.

## Project Overview
The core objective is to determine how digital connectivity (Internet Usage) correlates with economic output (GDP) and whether the growth rates of these two metrics show significant patterns over time.

1. Key Analysis Phases
- Data Cleaning & Preprocessing: Handling missing values using interpolation, forward-filling, and back-filling logic.
- Normalization of column headers and ensuring correct data types for years and financial metrics.

2. Feature Engineering:
- Categorizing countries into Developed (e.g., USA, UK, Germany, France, Japan) and Developing.
- Calculating year-over-year GDP Growth % and Internet Usage Growth %.
- Applying Log-transformation to GDP to ensure statistical stability during regression analysis.

3. Visualization:
- Line plots comparing internet usage trends between developed and developing nations.

4. Statistical Modeling:
- Running OLS (Ordinary Least Squares) Regression to analyze the impact of internet growth on economic performance.
- Diagnostic testing for Multicollinearity (VIF) and Heteroscedasticity (Breusch-Pagan/White tests).

## Requirements
To run this notebook, you will need the following Python libraries:
1. pandas
2. numpy
3. seaborn
4. matplotlib
5. statsmodels

## Dataset
The analysis expects a dataset.csv file located in a Google Drive directory (or local path). The required columns include:
- Country: Name of the nation
- Year: 2001 to 2024.
- Internet_Usage: Percentage of the population with internet access.
- GDP: Total Gross Domestic Product.

## Key Findings
- Usage Trends:
The gap between Developed and Developing nations in internet usage has significantly narrowed over the 2001–2024 period.
- Statistical Significance:
The regression model utilizes year-based fixed effects to account for global economic cycles.
- Model Diagnostics:
The analysis includes standard econometrics tests (Omnibus, Durbin-Watson) to ensure the validity of the regression results.

