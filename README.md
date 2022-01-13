# MechaCar_Statistical_Analysis
The data captured in the MechaCar_mpg.csv file reveals six measures recorded for the 50 prototype vehicles. A sample of the data is seen here:

![Car_Data_head](https://github.com/jp3tty/MechaCar_Statistical_Analysis/blob/main/Images/Car_Data_head.PNG)


## Linear Regression to Predict MPG

Using the linear regression capabilities of R, a model to predict mpg for prototype vehicles was developed as seen in the image below.

![Car_Data_linear_regression](https://github.com/jp3tty/MechaCar_Statistical_Analysis/blob/main/Images/Car_Data_linear_regression.PNG)

The results give the equations:

mpg = (6.267) VL + (0.0012) VW + (0.0688) SA + (3.546) GC - (3.411) AWD - 104.0.

where

VL = vehicle_length,
VW = vehicle_weight,
SA = spoiler_angle,
GC = ground_clearance,
AWD = AWD.

Statistical Summary:
![Car_Data_statistical_summary](https://github.com/jp3tty/MechaCar_Statistical_Analysis/blob/main/Images/Car_Data__statistical_summary.PNG)

From the statistical summary we see that:
* The vehicle length and ground clearance are likely to provide non-random amounts of variance in the model.


## Summary Statistics on Suspension Coils

![Coil_Data_head](https://github.com/jp3tty/MechaCar_Statistical_Analysis/blob/main/Images/Coil_Data_head.PNG)

![total_summary_df](https://github.com/jp3tty/MechaCar_Statistical_Analysis/blob/main/Images/total_summary_df.PNG)

![lot_summary_df](https://github.com/jp3tty/MechaCar_Statistical_Analysis/blob/main/Images/lot_summary_df.PNG)


## T-Tests on Suspension Coils

![ttest_all_lots](https://github.com/jp3tty/MechaCar_Statistical_Analysis/blob/main/Images/ttest_all_lots.PNG)

![ttest_for_each_lot](https://github.com/jp3tty/MechaCar_Statistical_Analysis/blob/main/Images/ttest_for_each_lot.PNG)

## Study Design: MechaCar vs Competition