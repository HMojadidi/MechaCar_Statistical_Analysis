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

# Deliverable 1: 
## Linear Regression to Predict MPG

![mpg_lin_reg_summary](https://user-images.githubusercontent.com/95712234/172521407-36bb666b-22e5-4298-af20-99077ceb8e69.png)

* Per the results, the most significant variables in our dataset which display a non-random effect on the mpg of the MechaCar are the Vehicle Length and the Ground Clearance. The linear regression model run on these variables againsts figures for mpg resulted in p-values of 2.60x10^-12 and 5.21x10^-8 respectively. The intercept was also statistically significant, indicating that there are likely other factors, not included in our dataset, that have a strong impact on the mpg.

* The slope of the linear model can not be considered to be zero, as the p-value of 5.35e-11, indicated by the orange arrow above, is lower than even an extreme level of significance, and thus the null hypothesis must be rejected. This means that the relationship between our variables and the miles per gallon is subject to more than random chance.

* This model predicts the mpg of the MechaCar prototype with some relative effectiveness. The r-squared value of 0.7149 indicates that the model is 71% accurate. There are still unconsidered factors in this model.


# Deliverable 2:
## Summary Statistics on Suspension Coils

![Susp_Coil_Total_Summary](https://user-images.githubusercontent.com/95712234/172527699-6f86ddf7-0fe1-4d37-bf83-8a559c40956d.png)
![Susp_Coil_Lot_Summary](https://user-images.githubusercontent.com/95712234/172527718-851c78fe-e136-494c-8c78-3ba60f2f5b2c.png)

While the overall variance, as shown in the Total Summary data above, is under 100 psi and meets specifications, there is a problem with one of the individual lots. As we can see in the Lot Summary stats, the variance for Lot 3 is well above the acceptable threshold, at 170.28.


# Deliverable 3:
## T-Tests on Suspension Coils

The Suspension Coil's PSI continuous variable across all manufacturing lots:


![Susp_Coil_One_Sample_ttest](https://user-images.githubusercontent.com/95712234/172530770-4364a0b9-64a6-46af-8806-aa0414558103.png)

The results of the T-test for the suspension coils across all manufacturing lots shows that they are not statistically different from the population mean, and the p-value is not low enough (0.06028) to reject the null hypothesis.

![Susp_Coil_Lot1_Samp_ttest](https://user-images.githubusercontent.com/95712234/172530905-8365536f-2654-4044-ae3f-5150f6e82aa9.png)

The results of the T-test for the suspension coils for Lot 1 shows that they are not statistically different from the population mean, and the p-value is not low enough (1) to reject the null hypothesis.

![Susp_Coil_Lot2_Samp_ttest](https://user-images.githubusercontent.com/95712234/172530926-08772240-c959-4c8e-a299-a2227ccae9d1.png)

The results of the T-test for the suspension coils for Lot 2 shows that they are not statistically different from the population mean, and the p-value is not low enough (0.6072) to reject the null hypothesis.


![Susp_Coil_Lot3_Samp_ttest](https://user-images.githubusercontent.com/95712234/172530944-ef3f120d-d449-4057-b93b-16321dfbc7cb.png)

The results of the T-test for the suspension coils for Lot 3 shows that they are slightly statistically different from the population mean, and the p-value is just low enough (0.0417) to reject the null hypothesis. This lot may need to be further evaluated.

# Deliverable 4:
## Study Design: MechaCar vs. Competition

In a world of rising fuel prices, global warming and a desire for budget efficiency, consumers are interested to know the fuel efficiency of a vehicle as part of their purchase decision. They will be looking to purchase a car who gives the most bang for the buck.

### Metric to test:

To find answers for ths test, we should evaluate MechaCar's fuel efficiency and compare it to the various competitor vehicles' fuel efficiency.

### Null and Alternate Hypothesis:

Ho: MechaCar prototypes' fuel efficiency is similar to competitor's vehicles in the same vehicle class.
Ha: MechaCar prototypes' fuel efficiency is statistically above or below that of vehicles in the same class.

### Statistical Test:

The two-sample t-tests would be ideal.

### Data Needed:

The test would need fuel efficiency data from the MechaCar Prototypes as well as from all major competitor vehicles. 

