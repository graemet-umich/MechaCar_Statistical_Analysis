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

![Linear Regression of MechaCar_mpg Data](./Resources/d2_dfs.png)
Fig. The total_summary (above) and lot_summary (below) dataframes.

## T-Tests on Suspension Coils


## Study Design: MechaCar vs Competition




When an intercept is statistically significant, it means that the intercept term explains a significant amount of variability in the dependent variable when all independent vairables are equal to zero. Depending on our dataset, a significant intercept could mean that the significant features (such as weight and horsepower) may need scaling or transforming to help improve the predictive power of the model. Alternatively, it may mean that there are other variables that can help explain the variability of our dependent variable that have not been included in our model. Depending on the dataset and desired performance of the model, you may want to change your independent variables and/or transform them and then re-evaluate your coefficients and significance.