# MechaCar_Statistical_Analysis

Project Objective
To analyze metrics that can affect the manufacturing of a new car prototype and compare vehicle performance across different manufacturer lots. These metrics include vehicle length, weight, spoiler angle, ground clearance, AWD capabilities, MPG, and PSI.

Liner Regression to Predict MPG
![image](https://user-images.githubusercontent.com/105396400/186569301-9a886f1f-b606-4caa-ba29-c9b7487b54f1.png)

3 Key Takeaways:

Variance of a non-random variable is usually 0. Given this fact, the intercept, vehicle_length, and ground_clearance coeeficients can be said to provide a non-random amount of variance to the mpg values.
At a significance level of 0.05, we are able to reject the null hypothesis because of the extremely small p-value. The null hypothesis of a linear regression states that the slope (β1) is equal to 0. However, if we reject the null hypthesis, we're stating that alternative (β1 ≠ 0) is true. Thus, proving that the slope is not 0.
Multiple R-squared increases as more variables are passed through the regression. However, adjusted R-squared controls against this increase, and adds penalties for the number of predictors in the model, thus making it a more accurate predictor of how effective the linear model is. An adjusted R-square of 0.6825 concludes that this linear model predicts the mpg of MechaCar prototypes relatively well.

Summary Statistics on Suspension Coils

![image](https://user-images.githubusercontent.com/105396400/186569648-2c534863-19b7-4039-8807-922f3aa946d1.png)
![image](https://user-images.githubusercontent.com/105396400/186569691-d0987c8e-6f10-41dd-8398-ff2131d756ae.png)
The overall variance for the entire dataset indicates that the current manufacturing data meets the 100 pounds per square inch variance limitation. However, when separated into three lots, the third lot demonstrates a much higher variance. Because the lots are chosen randomly, there is a possiblity that a third of the lot does not meet the necessary suspension coils requirement.

T-Tests on Suspension Coils

There is a summary of the t-test results across all manufacturing lots:
![image](https://user-images.githubusercontent.com/105396400/186570062-492bf424-4f1d-4804-90c0-8900c2e5607c.png)
From here we can see the true mean of the sample is 1498.78, which we also saw in the summary statistics above. With a p-Value of 0.06, which is higher than the common significance level of 0.05, there is NOT enough evidence to support rejecting the null hypothesis. That is to say, the mean of all three of these manufacturing lots is statistically similar to the presumed population mean of 1500.

Next looking at each individual lots:

Lot 1 sample actually has the true sample mean of 1500, again as we saw in the summary statistics above. With a p-Value of 1, clearly we cannot reject (i.e. accept) the null hypothesis that there is no statistical difference between the observed sample mean and the presumed population mean (1500).
Lot 2 has essentially the same outcome with a sample mean of 1500.02, a p-Value of 0.61; the null hypothesis cannot be rejected, and the sample mean and the population mean of 1500 are statistically similar.
However, Lot 3, not surprisingly is a different scenario. Here the sample mean is 1496.14 and the p-Value is 0.04, which is lower than the common significance level of 0.05. All indicating to reject the null hypothesis that this sample mean and the presumed population mean are not statistically different.

![image](https://user-images.githubusercontent.com/105396400/186570178-11cc663f-a670-4773-a028-bfbf9e75e108.png)
![image](https://user-images.githubusercontent.com/105396400/186570205-5a69e3a2-6fad-4b30-ba2b-241b51cef867.png)
![image](https://user-images.githubusercontent.com/105396400/186570238-2cb69e4a-dbd9-4bd0-a7d6-0f14925c9fa5.png)

Study Design: MechaCar vs. Competition

Another statistical study that can be performed to determine MechaCar's standing against its competition is a linear regression on city and highway fuel efficiency. Gasoline is expensive nowadays, and it is an important feature that many consumers look at when purchasing a new car. The metrics that can be included in this analysis are:

City and highway fuel efficiency: dependent variable
Horse power: independent variable
Vehicle weight: independent variable
AWD capabilities: independent variable
MPG: independent variable In addition to the MPG, AWD, and vehicle weight data that we already have, we would have to collect fuel efficiency and horse power data for the sample data set at hand.
