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






