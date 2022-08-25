# MechaCar_Statistical_Analysis

Project Objective
To analyze data points that hs the ability to alter the manufacturing of a new car prototype and compare vehicle metrics across different manufacturer vehicles. These metrics include vehicl, weight, spoiler angle, ground clearance, AWD capabilities, MPG, and PSI.

Liner Regression to Predict MPG
![image](https://user-images.githubusercontent.com/105396400/186569301-9a886f1f-b606-4caa-ba29-c9b7487b54f1.png)

3 Key Takeaways:

Variance of a non-random variable is usually 0. The intercept, vehicle_length, and ground_clearance coeeficients can provide a non-random amount of variance to the mpg values.
At a significance level of 0.05, we can reject the null hypothesis because of the extremely small p-value. The null hypothesis of a linear regression states that the slope is equal to 0. However, if we reject the null hypthesis, we're stating that alternative is true. Proving that the slope is not 0.
R-squared increases as more variables are passed through the regression. Adjusted R-squared controls against this increase, adds penalties for the number of predictors in the model, therefore making it a more accurate predictor of how effective the linear model is. An adjusted R-square of 0.6825 concludes this linear model predicts the mpg of MechaCar prototypes relatively well.

Summary Statistics on Suspension Coils

![image](https://user-images.githubusercontent.com/105396400/186569648-2c534863-19b7-4039-8807-922f3aa946d1.png)
![image](https://user-images.githubusercontent.com/105396400/186569691-d0987c8e-6f10-41dd-8398-ff2131d756ae.png)

The difference for the entire dataset shows that the current manufacturing data meets the 100 pounds per square inch difference limitation. However, when separated into three batches, the third batch shows a higher variance. Due to its randomness, there is a possiblity that a third of the batch does not meet the required suspension coils requirement.

T-Tests on Suspension Coils

![image](https://user-images.githubusercontent.com/105396400/186570062-492bf424-4f1d-4804-90c0-8900c2e5607c.png)

From here we can see the mean of the sample is 1498.78. With a p-Value of 0.06, which is higher than the common significance level of 0.05, there is not enough evidence in supporting the rejection of the null hypothesis. The mean of all three of these manufacturing batches is statistically similar to the presumed population mean.

Next looking at each individual lots:

Lot 1 sample actually has the true sample mean of 1500, same as what we saw in the summary statistics above. With a p-Value of 1, we cannot reject the null hypothesis that there is no statistical difference between the observed sample mean and the presumed population mean (1500).
Lot 2 has basically the same outcome with a sample mean of 1500.02, a p-Value of 0.06. The null hypothesis cannot be rejected, and the sample mean and the population mean of 1500 are statistically similar.
However, Lot 3 is different. Here the sample mean is 1496.14 and the p-Value is 0.04, which is lower than the common significance level of 0.05. All indicating that this sample mean and the presumed population mean are not statistically different.

![image](https://user-images.githubusercontent.com/105396400/186570178-11cc663f-a670-4773-a028-bfbf9e75e108.png)
![image](https://user-images.githubusercontent.com/105396400/186570205-5a69e3a2-6fad-4b30-ba2b-241b51cef867.png)
![image](https://user-images.githubusercontent.com/105396400/186570238-2cb69e4a-dbd9-4bd0-a7d6-0f14925c9fa5.png)

Study Design: MechaCar vs. Competition

An additional statistical analysis that can be undertaken to determine MechaCar's position against its competition is a linear regression on fuel efficiencies realted to city and highway travel. Fuel for vehicles is an important consideration that many consumers examine when purchasing a new car. The data that can be included in this analysis are:

Vehicle weight: independent variable
Horse power: independent variable
City and highway fuel efficiency: dependent variable
AWD capabilities: independent variable
MPG: independent variable 
