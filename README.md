# MechCar_Statistical_Analysis

## Overview 

A client has asked the data analytics team to determine what factors are causing the production team difficulties in completing their new prototype vehicle. We will examine the MPG and suspension in more detail and discover what if anything is a factor in their success.

## Linear Regression to Predict MPG (Deliverable 1)
In order to determine what, if any factors, had a correlation on MPG, the team ran a linear regression analysis on five components: vehicle length, vehicle weight, spoiler angle, ground clearance, and AWD. The overall P-Value of the linear regression was (5.3x10^-11) and this indicates that at least one factor has a correlation to the MPG of the prototype vehicle. In addition, the overall r-squared value was at .71 and this along with the overall P-Value indicate that the slope of the linear regression is not zero and that the data should be explored more.

Vehicle weight, spoiler angle, and AWD all had significance levels above the .05 threshold and therefore are not considered significant factors. Vehicle length and ground clearance did however have a P-Value score of smaller than .05 and must be considered, at least, measurable factors in the MPG of the prototype vehicle. The linear regression summary can be viewed below.

![Linear_regression.png](https://github.com/Brooks2210/MechCar_Statistical_Analysis/blob/main/Resources/Linear_regression.png)

## Summary Statistics on Suspension Coils (Deliverable 2)
In addition to the factors above, our client wanted us to examine the manufacturing of their suspension coils. In particular, the client wanted to make sure that the specifications, namely that the different lots did not exceed the 100 pounds per square inch variance and remained consistent for each production run.
In looking at the total summary of the suspension coil data, it clearly shows that the variance is less than the 100 pounds per square inch that the client expects, but given that the variance is 62, a closer look at the individual lots is warranted.

![Total_summary.png](https://github.com/Brooks2210/MechCar_Statistical_Analysis/blob/main/Resources/Total_summary.png)

As suspected, the individual lot summary gives a different picture. While Lot 1 and 2 have small variances, Lot 3 has a significant variance of 170 and deserves further examination.

![Lot_summary.png](https://github.com/Brooks2210/MechCar_Statistical_Analysis/blob/main/Resources/Lot_summary.png)

## T-Tests on Suspension Coils (Deliverable 3)

In analyzing the different lot data using a T-Test it becomes apparent that all the lots are not similar. Both Lot 1 and 2 have similar P-Values as the total summary P-Value, but Lot 3 has a P-Value of .15 and can be considered significantly different than the rest.

![Lot_1_2_3_t_test.png](https://github.com/Brooks2210/MechCar_Statistical_Analysis/blob/main/Resources/Lot_1_2_3_t_test.png)

## Study Design: MechaCar vs Competition (Deliverable 4)

The above analysis has given our client valuable insight into both their production process and what factors influence MPG. While all the analysis that was asked of us was completed, it would be helpful if our client also examined one other important factor in order to ensure future success, namely the role maintenance cost plays in the purchase decision of the consumer. 

Null Hypothesis: Maintenance cost do not factor in a consumer’s purchase of a vehicle.
In order to complete this analysis a detailed consumer survey will need to be created and randomly distributed to consumers that have recently purchased a vehicle.  
Once the surveys are complete, frequency data will then be used to run a chi-squared test to determine the frequencies across the different responses to the survey. While we will focus on the maintenance cost of the vehicle in determining the purchase of a vehicle, the other responses received in the survey may also prove to be just as valuable.
