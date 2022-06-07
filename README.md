# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

As per the results below, we can extract the following information:

The vehicle weight, spoiler angle, and All Wheel Drive (AWD) have p-Values that suggests a random amount of variance with data. Furthermore, we can also see that the vehicle length, and vehicle ground clearance are statistically likely to provide non-random amounts of variance to the model, since they have a significant impact on MPG (Miles per gallon) on the MechaCar prototype, also considering the intercept statistically there are many indicators that may have different factors not included on the dataset that would considerably impact on MPG.

Approaching the p-Value: 5.35e-11, the slope of the linear model cannot be considered zero, what brings us to conclude that our null hypothesis should be rejected, what translates to that the correlation between the variable presented and the miles per gallon are subjected to more than random chance.

Analyzing this linear model, the R-Squared value of 0.7149, translating to approximately 71% of total MPG prediction will be determined by the model prototype. In contrast of this information, we can assume that the effectiveness of 71% is high and considerable for further development. 

<img src="https://github.com/abramscris/MechaCar_Statistical_Analysis/blob/master/Images/MPG.png" width="700">

## Summary Statistics on Suspension Coils

At this point of the analysis, we examinate the Suspension Coil dataset we have filtered this information in one general data where we could identify that the variance of the coil is 62.29 PSI which is achieving expectations once the amount of 100 PSI was stablish as a variance requirement. 

<img src="https://github.com/abramscris/MechaCar_Statistical_Analysis/blob/master/Images/PSI.png" width="700">

But when we refine our search and divide the data within 3 Lots, we could clearly see that Lot 3 is significantly different than the standard 1500 PSI achieved by the Lot 1 and 2.

<img src="https://github.com/abramscris/MechaCar_Statistical_Analysis/blob/master/Images/Lot.png" width="700">

Considering the lower mean and high variance still on Lot, it can indicate that this lot is not consistent and under expectations in this comparation. You can visualize this information on the boxplot below:

<img src="https://github.com/abramscris/MechaCar_Statistical_Analysis/blob/master/Images/plot.png" width="500">
 
## T-Tests on Suspension Coils
Exploring the dataset of Suspension Coil it was performed t-tests in order to show statistical difference between the mean and a hypothetical population dataset of 1500.
On the tested performed we have found the following results:
The p-Value of 0.06 that is higher that significance level of 0.05, what presume that we do not have enough evidence to support a rejected of the null hypothesis once the mean of all the lots is similar statistically speaking when considered the population mean amount of 1500 as suggested.

<img src="https://github.com/abramscris/MechaCar_Statistical_Analysis/blob/master/Images/Coil1.png" width="700">

When looking specific to Lot 3 even though the p-Value is 0.04 on this test, indicating reject the null hypothesis, still is the lot that brings questions and differ from others. An inside look into the process of this lot would help understand the discrepancies and improvements needed.

<img src="https://github.com/abramscris/MechaCar_Statistical_Analysis/blob/master/Images/Lot3.png" width="700">

## Study Design: MechaCar vs Competition.
A more detailed statistical study for MechaCar could be approached analyzing a more specific data with the Top 10 better performed cars from the last 2 year following the additional metrics:

* MPG (Miles per gallon)
* Safety Features (front airbags, electronic stability control, safety belts and the LATCH child safety seat system)
* Selling Pricing

### Hypothesis: Null and Alternative

As we based our hypothesis on safety measures most requested on buying a car, we can have the following methods of hypotheses:

* Null Hypothesis (Ho): If MechaCar do not have the safety requirements as the TOP10 confirm if the selling price will be lower.
* Alternative Hypothesis (Ha): If MechaCar have the same safety requirements confirm if the price is lower or above.

### Statistical tests
The use of a multiple linear regression would be great determinant of the factors that have the highest correlation/predictability with the list selling price related to safety features and MPG, between more data provided.
