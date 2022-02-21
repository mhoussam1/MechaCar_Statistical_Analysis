# MechaCar_Statistical_Analysis


# Overview of Project:

This project involves the use of statistics and hypothesis testing to analyze a series of datasets from the automotive industry.
All of the statistical analysis and visualizations is written in the R programming language.


## Background: 

A few weeks after starting his new role, Jeremy is approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

In this challenge, you’ll help Jeremy and the data analytics team do the following:

Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
Run t-tests to determine if the manufacturing lots are statistically different from the mean population
Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.



# Linear Regression to Predict MPG

In the summary output, each Pr(>|t|) value represents the that each coefficient contributes a random amount of variance to the linear model as a probability. According to our results vehicle length and ground clearance provide a non-random amount of variance to the linear model of mpg.

![98474372-f439e280-21ba-11eb-8f80-d707ca8003d5](https://user-images.githubusercontent.com/93894964/154876523-3c9d0a0f-10ff-4e13-b550-da8b6a2bc85d.png)



### Multi linear model is:

mpg = 6.27 * vehicle_length + 1.25e-3 * vehicle_weigth + 6.88e-2 * spoiler_angle -3.41 * AWD + 3.55 * ground_clearance - 1.04e+2

R-square is 0.71 so 71% of the variations in mpg can be explained by changes in the vehicle length, the vehicle weight, the spoiler angle, the drivetrain and the ground clearance. We can consider this linear model as fairly efficient to predict mpg of MechaCar prototypes.

# Summary Statistics on Suspension Coils


All manufacturing lots:

![1](https://user-images.githubusercontent.com/93894964/154878019-f762add1-5846-4fb9-957c-fe4e21602f59.png)


By each manufacturing lot:

![2](https://user-images.githubusercontent.com/93894964/154878030-69eb6968-f2c5-4b7d-b6e4-f70ab97a2abd.png)




The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch.
The design specs are respected for all manufacturing lots in total with a global variance of 62.3 psi.
On the lot level, Lot 1 and Lot 2 are into specs with respectively variances of 0.98 and 7.5 psi. The Lot 3 is out of specs with a variance of 170.3 psi.



# T-Tests on Suspension Coils

## T-Test all manufacturing lots against the population mean

p-value of 0.069 is above the significance level. Therefore, we do not have sufficient evidence to reject the null hypothesis, and we can state that the PSI across all manufacturing lots is statiscally similar to the population mean of 1498.78 psi.

![3](https://user-images.githubusercontent.com/93894964/154878948-ffd06a7c-5393-4cfb-96e4-5a5a6d56bcb1.png)



## T-Tests each manufacturing lot against the population mean
