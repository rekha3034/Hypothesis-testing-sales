# Hypothesis-testing-sales

Hypothesis testing is a statistical method to determine if there is enough evidence in a sample of data to infer that a certain condition is true for the entire population. It is a type of statistical analysis in which you put your assumptions about a population parameter to the test. It is used to estimate the relationship between 2 statistical variables.
A hypothesis test examines two mutually exclusive claims about a parameter to determine which is best supported by the sample data. The parameter is usually the mean or proportion of some population variable of importance to the marketer.

Steps in Hypothesis Testing :

1.	Formulate Hypotheses
   
Null Hypothesis (H0):  is the default position that there is no relationship or no difference between the variables.  This hypothesis states that there is no effect or difference, and it is the hypothesis you attempt to reject with your test. 

Alternative Hypothesis (Ha):   The alternative or research hypothesis (HA) is the opposite of the null. This hypothesis is what you might believe to be true or hope to prove true. 

2.	Choose the Significance Level (α)
   
The significance level, often denoted by alpha (α), is the probability of wrongly rejecting the null hypothesis when it is true. The level is selected by the researcher and obtained by subtracting your confidence level from 100%. For instance, if you are 95% confident in your research, the alpha level will be 5% (0.05). Common choices for α are 0.05 (5%), 0.01 (1%), and 0.10 (10%).

3.	Select the Appropriate Test
   
Choose a statistical test based on the type of data and the hypothesis. Common tests include t-tests, chi-square tests, ANOVA, and regression analysis. The selection depends on data type, distribution, sample size, and whether the hypothesis is one-tailed or two-tailed.

4.	Collect Data
   
Gather the data that will be analyzed in the test. To infer conclusions accurately, this data should be representative of the population.

5.	Calculate the Test Statistic
    
Based on the collected data and the chosen test, calculate a test statistic that reflects how much the observed data deviates from the null hypothesis.

6.	Determine the p-value

The p-value is the probability of observing test results at least as extreme as the results observed, assuming the null hypothesis is correct. P-Value or probability value is a number that denotes the likelihood of your data having occurred under the null hypothesis of the statistical test.  It helps determine the strength of the evidence against the null hypothesis.

7.	Interpretation

Compare the p-value to the chosen significance level:

•	If the p-value ≤ α: Reject the null hypothesis, suggesting sufficient evidence in the data supports the alternative hypothesis.

•	If the p-value > α: Do not reject the null hypothesis, suggesting insufficient evidence to support the alternative hypothesis.

8.	Report the Results
    
Present the findings from the hypothesis test, including the test statistic, p-value, and the conclusion about the hypotheses.

**Types of Hypothesis Testing**

1.  **Z Test**
   
To determine whether a relationship between variables is statistically significant, hypothesis testing uses a z-test. It usually checks to see if two means are the same (the null hypothesis).  Z-test be applied only when the population standard deviation is known and the sample size is 30 data points or more.

2.  **T Test**
   
A statistical test called a t-test is employed to compare the means of two groups. To determine whether two groups differ or if a procedure or treatment affects the population of interest, it is frequently used in hypothesis testing.

One-tailed or two-tailed t test

•	Perform a two-tailed t test to test whether the two populations are different from one another

•	Perform a one-tailed t test to know whether one population mean is greater than or less than the other.

3.  **Chi-Square test**
 
Chi-square test analyzes the differences between categorical variables from a random sample to determine if the expected and observed results are well-fitted. It helps to determine whether a difference between two categorical variables is due to chance or a relationship between them.
There are two main types of Chi-Square tests :

a.   Test of Independence
   
The Chi-Square test of Independence is a inferential statistical test that examines whether the two sets of variables are likely to be related to each other or not. A relatively large sample size and independence of observations are the required criteria for conducting this test.

b.   Goodness-Of-Fit Test

In statistical hypothesis testing, the Chi-Square Goodness-of-Fit test determines whether a variable is likely to come from a given distribution. We must have a set of data values and an idea of the distribution of this data. This test demonstrates a way of deciding if the data values have a “ good enough” fit for our idea or if it is a representative sample data of the entire population. 

4.  **ANOVA**

ANOVA, or Analysis of Variance, is a statistical method used to compare the means of three or more groups.  For instance, in business, a company might use ANOVA to analyze whether three different stores are performing differently in terms of sales. It’s also widely used in fields like medical research and social sciences, where comparing group differences can provide valuable insights.

**Hypothesis Testing on the Bike Sales Data**

Hypothesis Testing is done to understand if there is a significant relationship between various variables in the sales data. By examining the dataset, the goal is to identify patterns and provide actionable insights for business decision-making.

Data Source: https://www.kaggle.com/datasets/heeraldedhia/bike-buyers  
Kaggle's dataset was used for this work. 

Feature description:

Categorical Features:
Marital_Status: 'Married', 'Single'
Gender: 'Female', 'Male'
Education: 'Bachelors', 'Partial College', 'High School', 'Partial High School', 'Graduate Degree'
Occupation: 'Skilled Manual', 'Clerical', 'Professional', 'Manual', 'Management'
Home_Owner: 'Yes', 'No'
Commute_Distance: 0.5, 2.5, 7.5, 10.0
Region: 'Europe', 'Pacific', 'North America'

Numerical Features: Income, Children, Age

Target feature: Purchased_Bike: 1, 0

Steps followed:

1.	Importing the dataset and performing exploratory data analysis to understand its structure and characteristics.
2.	Hypothesis testing helps to establish the association between the dependent variable, "Purchased_Bike," and independent variables like Income, Age etc.
3.	Setting up the Null Hypothesis (H0) and the alternate hypothesis (Ha).
4.	Checking assumptions of the test (Normality, Equal Variance). Use tools like histograms, Q-Q plots, or other statistical methods (optional).
5.	Setting a significance level (alpha).
6.	Calculating the test statistics and deciding on whether to accept or reject the null hypothesis.
7.	Drawing meaningful inferences from the analysis.
   
Findings:

-- Set the alpha = 0.05 (Significance Level)   

1.  Income and Bike Purchase:
   
Null Hypothesis (H0): There is no significant difference in mean income between those who purchased a bike and those who didn't.

Alternative Hypothesis (Ha): There is a significant difference in mean income between those who purchased a bike and those who didn't.

Mean Income (Purchased Bike): 57505.20 Mean Income (Did Not Purchase Bike): 54874.76 Standard Deviation of Income: 31066.07 

The Z-test was applied for hypothesis testing, and the results showed:
Z-statistic: 1.34 P-value: 0.1810 

Conclusion: Since P-value > 0.05, We do not reject the Null Hypothesis. There is no significant difference in mean income between those who purchased a bike and those who didn't.

2.  Age and Bike Purchase:
   
Null Hypothesis (H0): There is no significant difference in mean age between those who purchased a bike and those who didn't.

Alternative Hypothesis (Ha): There is a significant difference in mean age between those who purchased a bike and those who didn't.

Mean Age (Purchased Bike): 42.94 Mean Age (Did Not Purchase Bike): 45.35 Standard Deviation of Age: 11.35 

The Z-test was applied for hypothesis testing, and the results showed:
Z-statistic: -3.35 P-value: 0.0008 

Conclusion: since P-value < 0.05, we can reject the Null Hypothesis and conclude that there is a significant difference in mean age between those who purchased a bike and those who didn't.

3.  Children and Bike Purchase:

Null Hypothesis (H0): There is no significant difference in the proportion of individuals with no children who purchased a bike compared to those with 1-5 children who purchased a bike. 

Alternative Hypothesis (Ha): There is a significant difference in the proportion of individuals with no children who purchased a bike compared to those with 1-5 children who purchased a bike.

Chi square test for independence was applied.
Chi-square statistic: 0.78
P-value: 0.3757

Failed to reject the Null Hypothesis: There is no significant difference in the proportion of individuals with 0 children who purchased a bike compared to those with 1-5 children who purchased a bike.

4.  Gender and Bike Purchase:
     
Null Hypothesis (H0): There is no significant difference in the proportion of individuals who purchased a bike based on gender. There is no association between gender and bike purchase variables.

Alternative Hypothesis (Ha): There is significant difference in the proportion of individuals who purchased a bike based on gender. There is an association between gender and bike purchase.

Chi square test for independence was applied.
Chi-square statistic: 0.09 P-value: 0.7681

Conclusion: Sine P-value > 0.05, do not reject the Null Hypothesis and we can conclude that bike purchase is independent of gender. There is no significant difference in the proportion of individuals who purchased a bike based on gender.

5.  Marital Status and Bike Purchase:

Null Hypothesis (H0): Bike purchase is independent of marital status i.e. there is no association between marital status and bike purchase variables.

Alternative Hypothesis (Ha): There is an association between marital status and bike purchase variables.

Chi square test for independence was applied.
Chi-square statistic: 11.54 P-value: 0.0007
 
Conclusion: Since P-value is small, reject the Null Hypothesis and conclude that there is an association between Marital Status and bike purchase.

6.  Education and Bike Purchase:
   
Null Hypothesis (H0): Bike purchase is independent of education i.e. there is no association between education and bike purchase variables.

Alternative Hypothesis (Ha): There is an association between education and bike purchase.

Chi square test for independence was applied.
Chi-square statistic: 25.33 P-value: 0.0000

Conclusion: Reject the Null Hypothesis and conclude that there is an association between Education and bike purchase.

7.  Occupation and Bike Purchase: 

Null Hypothesis (H0): There is no significant difference in the proportion of individuals who purchased a bike based on their occupation. There is no association between occupation and bike purchase.

Alternative Hypothesis (Ha): There is significant difference in the proportion of individuals who purchased a bike based on their occupation. There is an association between occupation and bike purchase.

Chi square test for independence was applied.
Chi-square statistic: 8.01 P-value: 0.0914

Conclusion: Since P-value > 0.05, accept the Null Hypothesis. There is no significant difference in the proportion of individuals who purchased a bike based on occupation.

8.  Home Ownership and Bike Purchase:

Null Hypothesis (H0): There is no significant difference in the proportion of individuals who purchased a bike based on home ownership. There is no association between owning a house and bike purchase.

Alternative Hypothesis (Ha): There is significant difference in the proportion of individuals who purchased a bike based on home ownership. There is an association between owning a house and bike purchase.

Chi square test for independence was applied.
Chi-square statistic: 0.29 P-value: 0.5872

Conclusion: Failed to reject the Null Hypothesis. There is no association between owning a house and bike purchase.

9.Region and Bike Purchase
    
Null Hypothesis (H0): There is no significant difference in the proportion of individuals who purchased a bike based on their region. There is no association between region and bike purchase.

Alternative Hypothesis (Ha): There is significant difference in the proportion of individuals who purchased a bike based on region. There is an association between region and bike purchase.

Chi square test for independence was applied.
Chi-square statistic: 13.75 P-value: 0.0010

Conclusion: Reject the Null Hypothesis. There is an association between region and bike purchase.

10.  Cars and Bike Purchase:

Null Hypothesis (H0): Bike purchase is independent of no: of cars they owned i.e. there is no association between no: of cars and bike purchase.

Alternative Hypothesis (Ha): There is an association between no: of cars owned and bike purchase.

Chi square test for independence was applied.
Chi-square statistic: 52.94 P-value: 0.0000

Conclusion: Reject the Null Hypothesis. There is an association between the number of cars owned and bike purchase.

11.  Commute Distance and Bike Purchase:

Null Hypothesis (H0): Bike purchase is independent of commute distance i.e. there is no association between commute distance and bike purchase.

Alternative Hypothesis (Ha): There is an association between commute distance and bike purchase.

Chi square test for independence was applied. Chi-square statistic: 28.84 P-value: 0.0000

Conclusion: Reject the Null Hypothesis. There is an association between commute distance and bike purchase.



















