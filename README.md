# US-HOME-PRICES-IMPACT

Welcome to our "Exploring US Home Price Trends" project! We're diving into data to figure out what has been influencing home prices in the United States over the last 20 years. Using data and advanced techniques, we want to build a model that helps us understand how different factors relate to home prices. 

# THE TOOLS & LIBRARIES USED FOR THIS PROJECT:

- Programming Languages: Python
- Data Analysis Libraries: NumPy, pandas, matplotlib, seaborn
- Machine Learning Libraries: scikit-learn
- Data Visualization: Matplotlib, Seaborn
- Version Control: Git, GitHub
- Jupyter Notebooks for data exploration and analysis
  
# DATA COLLECTED:

The S&P U.S. Home Prices Index is influenced by various economic and demographic factors. Among the options you've listed, the main key factors that impact the S&P U.S. Home Prices Index include:

1. POPTHM (Population)
   - Changes in the population size and demographics can impact the demand for housing, subsequently influencing home prices.

2. GDP (Gross Domestic Product)
   - The overall economic performance, as measured by GDP, can affect consumer confidence, income levels, and housing demand, all of which impact home prices.

3. MORTGAGE RATE
   - Fluctuations in mortgage rates affect affordability, which in turn influences the demand for housing and housing prices.

4. HOUSING STARTS
   - The number of new housing units under construction reflects current and future supply in the housing market, impacting home prices.

5. MEDIAN SALES PRICE
   - This directly reflects changes in the prices of homes sold within the market and serves as an indicator of market conditions.

6. HOMEOWNERSHIP RATE
   - Changes in the homeownership rate can influence the balance of supply and demand in the housing market, impacting home prices.

7. UNEMPLOYMENT RATE
   - Employment and income levels impact the ability and willingness of individuals to purchase homes, thus affecting home prices.

These key factors play significant roles in influencing the S&P U.S. Home Prices Index and are important considerations for understanding the dynamics of the housing market.
# FEATURE SELECTION:
In our analysis, we found certain important characteristics that are closely related to the S&P Home Price Index.   

 
 
 When a correlation value is positive, it means there is a direct relationship with home prices, while negative values indicate an inverse relationship. Features with higher absolute correlation values have a bigger impact on home prices.
 
# MODEL SELECTION & CROSS_VALIDATION:

we have two best models for US home prices one is linear regression another one is lasso regression 

In this project, we used the Lasso regression model to address significant collinearity within the dataset. The Lasso model employs L1 regularization to handle collinearity, promoting sparsity in feature coefficients.

To enhance the Lasso model's performance and determine the best regularization hyperparameter (alpha), we conducted cross-validation.

The optimal alpha value was found to be 0.0001 
During cross-validation, the R-squared scores for different folds were as follows:

Fold 1: 0.9384

Fold 2:-0.0281

Fold 3: 0.9457

Fold 4: 0.7558

Fold 5: 0.8689

* mean R_squared:0.6961
* standard deviation on R_squared:0.3685
  
# BEST FEATURES WITH NON_ZERO_COEFFICIENTS:

Our Lasso regression model identified certain features with non-zero coefficients:


signifying their impact on predicting home prices.
Positive coefficients indicate a direct relationship with home prices, while negative coefficients suggest an inverse relationship.

# FEATURES WITH ZERO_COEFFICIENTS :

In our analysis, we found that one features had coefficients of 0.0,

this features  do not have a significant impact on the prediction of home prices in our model.

# SOURCE
https://fred.stlouisfed.org/
