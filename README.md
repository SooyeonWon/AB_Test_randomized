# A/B Test for Randomized Design: Website Conversion Rates
#### by Sooyeon Won 

## Introduction
For this project, I worked to understand the results of an A/B test run by an e-commerce website, as the project of _Data Analyst Statistics_ in [Udacity Nanodegree Program for Data Analytics](https://www.udacity.com/course/data-analyst-nanodegree--nd002).  The company has developed a new web page in order to try and increase the number of users who "convert," meaning the number of users who decide to pay for the company's product. The goal is to help the company understand whether they should implement this new page, keep the old page, or perhaps run the experiment longer to make their decision.
<br><br>

## Summary of Findings
This analysis focuses mainly on the business decision, whether an e-commerce company should implement the new page design in its website to increase conversion rate. The users are randomly assigned to either control or treatment group. The users in both groups show very similar patterns of visiting the company's web page. The only difference between the two groups is the type of landing page. Old, new page design is assigned to the users in control, treatment group, respectively. The experiment is run for 23 days. This analysis investigated the influence of new webpage through (1)probability comparison, (2)A/B test and (3)regression approach. <br><br>
   1. **Probability Comparison** <br>
   First, I simply compared the conversion rate between the two groups. The overall conversion rate is 0.1196. The proportion of converted users in control group, in treatment group is 0.1204, 0.1188, respectively. The convert rate for control group is slightly higher than the other group users. However, the small difference could be occurred due to sampling errors. Thus, I conducted an additional test: A/B Test. <br><br>
   2. **A/B Test**<br>
   Second, I started with the idea that the convert rate for old page group is better or at least equal to that for new page group($H_0$). However, the p-value from 2 samples proportion-based z-test indicates that we do not have sufficient evidence to reject the null hypothesis. This finding corresponds to the results from regression analysis. <br><br>
   3. **Regression Analysis**<br>
   Finally, the regression results show that the treatment group is 1.0151 times **less** likely to convert a user than the control group, holding all else in the model constant. As the earlier findings, the difference of conversion rates for both groups are exceedingly small, and the associated p-value indicates that the coefficient is statistically insignificant. The outcomes from the regression approach support the previous conclusion that we fail to reject the idea that the convert rate for old page users is better than or equal to the rate for new page users. 
<br><br>

## Key Insights for Presentation

The findings from the three analysis are consistent. We can not reject the fact that user convert rate for old page is better than or at least is equal to the rate for new page. Therefore, the company should keep the old page, rather than implementing their new page. <br><br>

## References 
- [Two-proportion z-test](https://sonalake.com/latest/hypothesis-testing-of-proportion-based-samples/) 
- [Logistic Regression](https://www.statsmodels.org/stable/generated/statsmodels.discrete.discrete_model.Logit.html)
- [Regression Hypothesis](https://statisticsbyjim.com/regression/interpret-coefficients-p-values-regression/)
- [Multiple Linear Regression](https://onlinelibrary.wiley.com/doi/pdf/10.1197/j.aem.2003.09.006#:~:text=Multiple%20linear%20regression%20allows%20the,individual%20factor%20with%20the%20outcome.)
