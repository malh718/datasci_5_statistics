# datasci_5_statistics

## 1. Chi-Square Test: R 
Hypothesis 
X-squared = 14363, df = 1, p-value < 2.2e-16

There is an association between providers who can order Durable Medical Equipment in hospitals  and providers who are also covered under Medicare Part B and have the DME benefits covered. 

My null hyptohesis would be that there is no correlation between the two categories and they are not related whatsoever. 

In this case, my p value is 2.2e-16 which is less than .05 so the null hypthesis can be rejected in this case. 2.2e-16 is a very small number and since the P-value is less than the 5% significant or .05, the null hypthesis will be ignored.

## 2. T-Test:

In this situation the key chronic disease I chose was Cancer. In this case my hypothesis is that states other than northern states have a higher chance of cancer than northern states. What this means is that I believe people from the south have higher cancer incidence than people in the north. In this case my null hypothesis would be that there is no correlation whatsoever for location and its effect on cancer, and that they are both the same. 

The results of the t-test are as follows.
	Welch Two Sample t-test

data:  south and other
t = 1.1297, df = 40.586, p-value = 0.2652
alternative hypothesis: true difference in means is not equal to 0
95 percent confidence interval:
 -0.002269783  0.008028606
sample estimates:
 mean of x  mean of y 
0.08236471 0.07948529 


The welch t-test compares two areas we wanted to look at. Southern states and other states. The t value is 1.129 and the p value is .2652. The mean for the information for cancer in the south is higher than that of the mean of the other, which is .0823 and .0794. What this shows is that the south is a little bit higher than other areas, but not by alot . However since the p value is .26 which is  higher than .05 we cant reject the null hypthesis. 



## 3. ANOVA:

I tried 3 different csv files to figure out the ANOVA test however I kept getting the same error. Error in eval(predvars, data, env) : object 'diet6weeks' not found. And then it showed a number of different traceback errors. It was at this point that I decided to redo the class assgignment, and even though it had worked during class it still showed a traceback error. I was confused by this because my class code worked prior, and I even tried refreshing my computer. Still an error showed. I found a very basic CSV file to test this anova out, that had to do with block, color and response. Still there was an error. However, then my laptop died and when it was charged it started working. All three examples that I had created went through with the summaries.  Also at the end of the code, instead of setting it equal to opioids, I just put the name of the dataset and it worked. My numbers did match up with the class numbers and the code ran. 

class example

<img width="552" alt="Screen Shot 2023-10-13 at 2 45 46 PM" src="https://github.com/malh718/datasci_5_statistics/assets/102617334/d8089989-73ff-4d18-a58c-91e4f5d84220">



For the class example the we are looking at the overall opioid and its relationship to two independent variables, which are rural_urban and payer. 

Basic color example 
Df Sum Sq Mean Sq
block       23  779.8    33.9
color        1  437.6   437.6
block:color 23  395.1    17.2

diet example
<img width="542" alt="Screen Shot 2023-10-13 at 2 46 00 PM" src="https://github.com/malh718/datasci_5_statistics/assets/102617334/3bab9c04-f6bd-4f1e-9efd-2eaf17f225da">


My hypothesis for this diet example would be the average weight lost after a period of 6 weeks varies across patients who are in different age and height groups. In this case the weight6weeks is the dependent variable and the age and height are independent variables.  The dataset for this example is called an2. The p value for height is less than .05 and is .037. This shows that height does affect weight6weeks which is weightloss after 6 weeks. The statistics show that afge is not as significant with a p value of .747. 




## 4. Regression Analysis:

I started off doing some practice with the example that was provided in class with the hospital and employees on payroll with the number of beds. That showed me a summary of model6, which shows a multple r-squared to be.7161 and the standard of error to be 416.5. The P and F value are as follows. F-statistic: 1.259e+04 on 1 and 4993 DF,  p-value: < 2.2e-16. 

My hypothesis for this example is that we are looking at how the number of beds is related to the full time equivalent of employees on the payroll. As the graph shows the linear regression that the more beds there are the more employees that are gonna have to be on working full time. 

This was also proven by the graph that was populated. 
<img width="428" alt="Screen Shot 2023-10-13 at 3 13 23 PM" src="https://github.com/malh718/datasci_5_statistics/assets/102617334/e645e8c3-d121-4a8c-aa55-e12a5455014c">



I followed the class example with a linear regression based on some salary data. My code read model8 <- lm(df8$YearsExperience ~ df8$Salary)
summary(model8) and it showed that the statistics are as follows 
Residual standard error: 0.5992 on 28 degrees of freedom
Multiple R-squared:  0.957,	Adjusted R-squared:  0.9554 
F-statistic: 622.5 on 1 and 28 DF,  p-value: < 2.2e-16. 

My hypothesis for this linear regression would be that the more years experiance you have, the better your salary will be. The null hypothesis would be that they have no correlation whatsoever. The p value present in this example is much lower than .05, and the p value as mentioned above is 2.2e-16. This shows that there is a signficant relationship between YearsExperience and Salary. The direction indicated that the sign of the coefficient for Years of experiance is positive which means as salary increases so does experience. The r value in this example is also high, it is .957 which is very close to one. What this means is that this is strong and has a strong relationship.

 <img width="420" alt="Screen Shot 2023-10-13 at 3 20 52 PM" src="https://github.com/malh718/datasci_5_statistics/assets/102617334/2fe9530b-5e79-42b6-a92a-a698eb793f51">


