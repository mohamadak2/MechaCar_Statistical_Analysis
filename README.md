# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

Call:
lm(formula = mpg ~ vehicle_length + vehicle_weight + spoiler_angle + 
    ground_clearance + AWD, data = df)

Residuals:
     Min       1Q   Median       3Q      Max 
-19.4701  -4.4994  -0.0692   5.4433  18.5849 

Coefficients:
|                 |  Estimate Std. | Error t    | t value | Pr(>\|t\|)   |
| :---:           | :---:          | :---:      | :---:   | :---:        |
|(Intercept)      | -1.040e+02     |  1.585e+01 | -6.559  | 5.08e-08 *** |
|vehicle_length   |  6.267e+00     | 6.553e-01  | 9.563   | 2.60e-12 *** |
|vehicle_weight   |  1.245e-03     | 6.890e-04  | 1.807   | 0.0776 .     |
|spoiler_angle    |  6.877e-02     | 6.653e-02  | 1.034   | 0.3069       |
|ground_clearance |  3.546e+00     | 5.412e-01  | 6.551   | 5.21e-08 *** |
|AWD              | -3.411e+00     | 2.535e+00  | -1.346  | 0.1852       |
---
Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

| Residual standard error: | 8.774 on 44 degrees of freedom |
| :---                     | :---                           |
| Multiple R-squared:      | 0.7149                         |
|Adjusted R-squared:       | 0.6825                         |
|F-statistic:              | 22.07 on 5 and 44 DF           |
|p-value:                  | 5.35e-11                       |


#
**Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?**

    The following variables provided a non-random amount of variance to the mpg:
    - (Intercept)
    - vehicle_length
    - ground_clearance

**Is the slope of the linear model considered to be zero? Why or why not?**
 
    The slope of this linear model is not considered to be zero because at least one of the variables provided a non-random amount of variance.


**Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?**

    Yes this linear model can predict the mpg of a car effectively. This is becase the R- squared is 0.7149. This means around 70% of the time mpg can be predicted.

#



#D3

**data:  suspension_coil_table$PSI**
t = -1.8931, df = 149, p-value = 0.06028
alternative hypothesis: true mean is not equal to 1500
95 percent confidence interval:
 1497.507 1500.053
sample estimates:
mean of x 
  1498.78
  
**t.test(psisubsetlot1$PSI, mu = 1500)**

	One Sample t-test

data:  psisubsetlot1$PSI
t = 0, df = 49, p-value = 1
alternative hypothesis: true mean is not equal to 1500
95 percent confidence interval:
 1499.719 1500.281
sample estimates:
mean of x 
     1500 

**t.test(psisubsetlot2$PSI, mu = 1500)**

	One Sample t-test

data:  psisubsetlot2$PSI
t = 0.51745, df = 49, p-value = 0.6072
alternative hypothesis: true mean is not equal to 1500
95 percent confidence interval:
 1499.423 1500.977
sample estimates:
mean of x 
   1500.2 

**t.test(psisubsetlot3$PSI, mu = 1500)**

	One Sample t-test

data:  psisubsetlot3$PSI
t = -2.0916, df = 49, p-value = 0.04168
alternative hypothesis: true mean is not equal to 1500
95 percent confidence interval:
 1492.431 1499.849
sample estimates:
mean of x 
  1496.14 
  
  
   #
   
   ## Study Design: MechaCar vs Competition
   
   ### Description

In our analysis we reviewed the following components:
- PSI
- Manufactured Lot #
H0 : There is no statistical difference between the Manufactured Lot # and their PSI its presumed population mean 1500.
Ha : There is a statistical difference between the Manufactured Lot # and its PSI presumed population mean 1500.

