# MechaCar_Statistical_Analysis
The data captured in the MechaCar_mpg.csv file reveals six measures recorded for the 50 prototype vehicles. A sample of the data is seen here:

![Car_Data_head](https://github.com/jp3tty/MechaCar_Statistical_Analysis/blob/main/Images/Car_Data_head.PNG)


## Linear Regression to Predict MPG

Using the linear regression capabilities of R, a model to predict mpg for prototype vehicles was developed as seen in the image below.

![Car_Data_linear_regression](https://github.com/jp3tty/MechaCar_Statistical_Analysis/blob/main/Images/Car_Data_linear_regression.PNG)

The results give the equations:

mpg = (6.267) VL + (0.0012) VW + (0.0688) SA + (3.546) GC - (3.411) AWD - 104.0.

where

* VL = vehicle_length,
* VW = vehicle_weight,
* SA = spoiler_angle,
* GC = ground_clearance,
* AWD = AWD

Statistical Summary:

![Car_Data_statistical_summary](https://github.com/jp3tty/MechaCar_Statistical_Analysis/blob/main/Images/Car_Data__statistical_summary.PNG)

From the statistical summary we see that:
* The vehicle length and ground clearance coeeficients are likely to provide non-random amounts of variance in the model due to their low p-values. This indicates that the variance of a MechaCar's vehicle length and groud clearance coefficients will meaningfully impact mpg.
* With a significance level of 0.05, we can consider the slope of the linear model to be zero and reject the null hypothesis due to very low p-value of 5.35e-11.
* An R-squared value of 0.7149 indicates that roughly 72% of mpg predictions will be correct using the linear model listed above. Generally, a higher R-squared value will inspire more confidence in a linear regression model, but with some experience in the subject matter this value should be adequate.


## Summary Statistics on Suspension Coils

Another dataset contains vehicle measurements from multiple production lots. Weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots.

A sample of the Suspension Coil data:

![Coil_Data_head](https://github.com/jp3tty/MechaCar_Statistical_Analysis/blob/main/Images/Coil_Data_head.PNG)


Summary of the Suspension Coil data:

![total_summary_df](https://github.com/jp3tty/MechaCar_Statistical_Analysis/blob/main/Images/total_summary_df.PNG)

The overall summary of the of the entire population show that the variance of the coils is 62.29 PSI, which is well within the 100 PSI variance requirement.


Summary of the Suspension Coil data by Lot Number:

![lot_summary_df](https://github.com/jp3tty/MechaCar_Statistical_Analysis/blob/main/Images/lot_summary_df.PNG)

An investigation of each lot reveals that Lot 1 and Lot 2 are well within the 100 PSI variance requirement, with variances of 0.98 and 7.47 respectively. Lot 3, however, has a disproportionately larger variance of 170.29.
 

## T-Tests on Suspension Coils

T-Test summary for all manufacturing lots:

![ttest_all_lots](https://github.com/jp3tty/MechaCar_Statistical_Analysis/blob/main/Images/ttest_all_lots.PNG)

The mean of all three manufacturing lots is statistically similar according to the summary above. The true mean of the sample is 1498.78 and the p-value is 0.06, which is higher than a common significance level of 0.05. This indicates that there is not enough evidence to support rejecting the null hypothesis.


T-Test summary for each lot:

![ttest_for_each_lot](https://github.com/jp3tty/MechaCar_Statistical_Analysis/blob/main/Images/ttest_for_each_lot.PNG)

From the summary for each lot, shown above, we see that Lot 1 and 2's sample mean, 1500 and 1500.2 respectively, are close to the presumed population mean, 1500, and their p-values are higher than a common significance 0.05. Indicating that we cannot reject the null hypothesis.

Lot 3, on the other hand, has a sample mean of 1496.14 and a p-value of 0.04168, which is lower than the common significance. In this case the null hypothesis that the sample mean and the presumed poputlation mean are not statistically different and should be rejected.

## Study Design: MechaCar vs Competition

An additional statistical study to quantify MechaCar's performance against their competitors 
* City and highway fuel efficiency
* Horse power
* Vehicle weight
* AWD capabilities
* MPG


