# A/B test
**Description:** This work involves analyzing the data of a large online store. Together with the marketing department, a list of hypotheses is being analyzed to increase revenue. The result of the work is the prioritization of hypotheses, conducting an A/B test, and interpreting its results.
**Main aims:** 
1. Prioritization of given hypothesis.
2. A/B test results interpretation with provision of recommendations.

### Table of Contents

- Introduction
  - Description.
  - Main aims.
  - Data description.
- Preparation
  - Importing libs.
  - Data import, research and preparation.
- Prioritization of hypotheses
  - Applying framework ICE for prioritization.
  - Applying framework RICE for prioritization.
  - Interpretation of the application of frameworks.
- A/B testing
  - Exploration of data.
  - Exploration of cumulative revenue by groups.
  - Analysis of cumulative average check by groups.
  - Relative change in cumulative average check of Group B compared to Group A.
  - Cumulative average number of orders per users by groups.
  - Relative change of cumulative average number of orders per user of Group B to Group A.
  - Scatter plot of the number of orders per user.
  - Calculating the 95th and 99th percentiles of the number of orders per user.
  - Scatter plot of revenue from orders.
  - 95-th and 99-th percentile of order value.
  - Calculation of statistical significance of differences in the average number of orders per visitor between groups based on "raw" data.
  - Calculation of statistical significance of the differences in the average order value between groups based on "raw" data.
  - Calculation of the statistical significance of differences in the average number of orders per visitor between groups based on "clean" data.
  - Calculation of the statistical significance of the differences in the average order value between the groups based on "clean" data.
- Results

### Interpretation of the application of frameworks 
For the purpose of prioritizing hypotheses, two frameworks were used: ICE and RICE. The difference between the frameworks is that RICE takes into account an important element called Reach, which reflects the degree of user coverage during hypothesis testing.

* According to the ICE framework, the most promising hypothesis is hypothesis #9, but due to low user coverage (Reach equals 1), RICE reduces its priority.
* Both frameworks indicate the potential of hypothesis #8 (mainly due to a coverage score of 10) and hypothesis #1 (with an impact score of 10).
* Hypothesis #7, due to low testing costs and high confidence in the results according to both frameworks, is evaluated at a relatively high level.


### A/B test results interpretation:
* Significant differences between groups A and B in the average number of orders. Group B has a 19% higher rate on "clean" data;

<p align="center">
  <img src="https://github.com/AntonMiniazev/YaP_projects/blob/main/4.%20Online_Retail_AB_test/imgs/Orders.png" />
</p>

* No significant differences between groups A and B in the average check. Group A had a 28.7% lower rate on "raw" data, but higher by 2.2% on "clean" data. The above conclusions obtained using the Mann-Whitney criterion were obtained both on "raw" and "clean" data. 
 
The need to clean the data was also confirmed by the significant difference in the average check between the groups: there were abnormally high checks in group B that distorted the mean values.

<p align="center">
  <img src="https://github.com/AntonMiniazev/YaP_projects/blob/main/4.%20Online_Retail_AB_test/imgs/Check.png" />
</p>

<b>Proposal based on the analysis above:</b> record the test results and designate group B as the winner. Despite the minor differences in the check, group B shows a significantly better number of orders.

