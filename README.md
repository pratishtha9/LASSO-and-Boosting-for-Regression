# LASSO-and-Boosting-for-Regression
Many variables are included so that algorithms that select or learn weights for attributes could be tested. However, clearly unrelated attributes were not included; attributes were picked if there was any plausible connection to crime (N=122), plus the attribute to be predicted (Per Capita Violent Crimes). The variables included in the dataset involve the community, such as the percent of the population considered urban, and the median family income, and involving law enforcement, such as per capita number of police officers, and percent of officers assigned to drug units.

The per capita violent crimes variable was calculated using population and the sum of crime variables considered violent crimes in the United States: murder, rape, robbery, and assault. There was apparently some controversy in some states concerning the counting of rapes. These resulted in missing values for rape, which resulted in incorrect values for per capita violent crime. These cities are not included in the dataset. Many of these omitted communities were from the midwestern USA.

1. Pre-processed the Communities and Crime Dataset to deal with missing values by using the “Mean Substitution” technique of data imputation.

2. Plotted a covariance matrix heatmap to identify the strongest correlation between the predictors (population, number of homeless people, number of immigrants, number of people living in urban areas, etc.) and the label (Violent Crimes per population). 

3. Selected top 11 features responsible for violent crimes in a community by looking at their coefficient of variation values. Created scatter plots and box plots to give more insight about the dataset using matplotlib and seaborn libraries.

4. Compared the performance of Linear regression, Ridge regression, LASSO regression and Principle component regression models on the dataset to find the best fit.

5. Achieved a lowest test error rate of 1.69% in the XGBoost Model using L1 penalised linear regression. 
