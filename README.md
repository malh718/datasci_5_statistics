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
class ex

### Df  Sum Sq Mean Sq F value Pr(>F)    
payer                4  957764  239441   76.42 <2e-16
rural_urban          1  535719  535719  170.97 <2e-16 
payer:rural_urban    4  380542   95135   30.36 <2e-16 
Residuals         1904 5965898    3133                   
---


For the class example the we are looking at the overall opioid and its relationship to two independent variables, which are rural_urban and payer. 

Basic color example 
Df Sum Sq Mean Sq
block       23  779.8    33.9
color        1  437.6   437.6
block:color 23  395.1    17.2

### diet example 
Df Sum Sq Mean Sq F value Pr(>F)  
Age          1      8     7.7   0.104  0.747  
Height       1    332   332.3   4.491  0.037 
Age:Height   1    182   182.3   2.464  0.120  
Residuals   86   6363    74.0                 
---
Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

My hypothesis for this diet example would be the average weight lost after a period of 6 weeks varies across patients who are in different age and height groups. In this case the weight6weeks is the dependent variable and the age and height are independent variables.  The dataset for this example is called an2. The p value for height is less than .05 and is .037. This shows that height does affect weight6weeks which is weightloss after 6 weeks. The statistics show that afge is not as significant with a p value of .747. 











