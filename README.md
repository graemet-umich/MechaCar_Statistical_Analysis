# MechaCar_Statistical_Analysis
Statistics and R

## Linear Regression to Predict MPG

The variables/features that provide a non-random amount of variance, i.e. those with significant p-values, are vehicle_length, ground_clearance, and intercept.

The slope of the linear model is non-zero, because the coefficients of vehicle_length (6.27) and ground_clearance (3.55) are non-zero.

The model is relatively effective in predicting the mpg of MechaCar prototypes, as the model explains 71% (Multiple R-squared = 0.71) of the variance of mpg. However, the significance of the intercept may mean that the significant features need transforming or that other features not included in the regression need to be included to improve the predictive power of the model.

![Linear Regression of MechaCar_mpg Data](./Resources/d1_lm.png)
Fig. Multiple linear regression on how mpg varies with vehicle_length, vehicle_weight, spoiler_angle, ground_clearance, and AWD.

## Summary Statistics on Suspension Coils

"The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch."

- **total_summary.** The total_summary shows that the combined Lot variance is 62.3 pounds per square inch, which is within the design specifications.

- **lot_summary.** However, the lot_summary shows that Lot1 (variance = 0.980 pounds per square inch) and Lot2 (variance = 7.47 pounds per square inch) are within the design specifications, but Lot3 (variance = 170 pounds per square inch) exceeds the design specifications of 100 pounds per square inch.

![Summary Statistic on All Lots and Each Lot](./Resources/d2_dfs.png)
Fig. The total_summary (above) and lot_summary (below) dataframes.

## T-Tests on Suspension Coils

One sample t-tests are used, because the comparison is between the mean of the population and the mean of a sample of that population. The mean of all Lots (1498.78, n=150, p=0.060), the mean of Lot1 (1500, n=50, p=1), and the mean of Lot2 (1500.2, n=50, p=0.607) are not significantly different from the population mean (1500). However, the mean of Lot3 (1496.14, n=50, p=0.042) is significantly different from the population mean (1500).

![All Lots v Population](./Resources/d3_tot.png)
Fig. t-test: mean of all Lots v. mean of population.

---
![Lot1 v Population](./Resources/d3_lot1.png)
Fig. t-test: mean of Lot1 v. mean of population.

---
![Lot1 v Population](./Resources/d3_lot2.png)
Fig. t-test: mean of Lot2 v. mean of population.

---
![Lot1 v Population](./Resources/d3_lot3.png)
Fig. t-test: mean of Lot3 v. mean of population.

## Study Design: MechaCar vs Competition


