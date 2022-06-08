# MechaCar_Statistical_Analysis

Using statistical analysis with R to analyze automobile performance

# Overview

AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. The data analytics team has been asked to review the production data for insights that may help the manufacturing team.

In this project, I will:

* Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes

* Collect summary statistics on the PSI of the suspension coils from the manufacturing lots

* Run t-tests to determine if the manufacturing lots are statistically different from the mean population

* Design a study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers with a summary interpretation of the findings.

# Results


![mpg_lin_reg_summary](https://user-images.githubusercontent.com/95712234/172521407-36bb666b-22e5-4298-af20-99077ceb8e69.png)

* Per the results, the most significant variables in our dataset which display a non-random effect on the mpg of the MechaCar are the Vehicle Length and the Ground Clearance. The linear regression model run on these variables againsts figures for mpg resulted in p-values of 2.60x10^-12 and 5.21x10^-8 respectively. The intercept was also statistically significant, indicating that there are likely other factors, not included in our dataset, that have a strong impact on the mpg.

* The slope of the linear model can not be considered to be zero, as the p-value of 5.35x10^-11, indicated by the orange arrow above, is lower than even an extreme level of significance, and thus the null hypothesis must be rejected. This means that the relationship between our variables and the miles per gallon is subject to more than random chance.

* This model predicts the mpg of the MechaCar prototype with some relative effectiveness. The r-squared value of 0.7149 indicates that the model is 71% accurate. There are still unconsidered factors in this model.


# Summary Statistics on Suspension Coils

![Susp_Coil_Total_Summary](https://user-images.githubusercontent.com/95712234/172527699-6f86ddf7-0fe1-4d37-bf83-8a559c40956d.png)
![Susp_Coil_Lot_Summary](https://user-images.githubusercontent.com/95712234/172527718-851c78fe-e136-494c-8c78-3ba60f2f5b2c.png)







