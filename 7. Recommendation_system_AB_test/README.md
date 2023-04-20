# Recommendation system AB test
**Description:** Analysis of the result of A/B test on the service that tried to implement an improved recommendation system. Expected results were to improve the conversion metrics within 14 days from the registration date.
**Main aims:** 
Evaluation of the results of A/B test according to the statement of work:
- Test name: recommender_system_test;
- Groups: A - control group, B - new payment funnel;
- Launch date: 2020-12-07;
- Date of stopping the acquisition of new users: 2020-12-21;
- Test stop date: 2021-01-04;
- Audience: 15% of new users from the EU region;
- Test purpose: testing changes related to the implementation of an improved recommendation system;
- Expected number of test participants: 6000.
- Expected effect: within 14 days from the registration date, users will show an improvement in each metric by at least 10%:
  - conversions to product page views - product_page event,
  - product cart views - product_cart,
  - purchases - purchase.

### Table of Contents

- Introduction
  - Description
  - Main aims
  - Data description
- Preparation
  - Importing libs
  - Data import, research and preparation
- Evaluation of the correctness of the test
  - Checking for overlap between the test audience and the competing test, as well as within groups
  - Checking the match of the test and marketing events
  - Checking for other issues with the temporal boundaries of the test
  - Checking the proportion of new users by regions
  - Checking the distribution of users among groups
- Exploration data analysis
  - Distribution of users across test groups
  - Distribution of the number of events per user
- Analysing test results
  - Conversion in the funnel by stage
  - Checking the statistical difference of proportions with the z-test
- Results and recommendations

### Results and recommendations
The initial data had the following problems:

- The stop date for the acquisition of new users did not match the statement of work;
- There was a lack of logs to evaluate the effects for 14 days for the entire sample;
- Due to the need to comply with the 14-day measurement, the sample size was reduced to less than the expected number of participants by 6000;
- The test was affected by marketing activities and the New Year holiday period.

These problems could significantly distort the results of the analysis, but the obtained data rather indicate that the improvements did not show the expected result not because of errors in the data, but because of the changes made. I suggest considering the test successful.

As a result of studying the resulting sample, it can be concluded that the measured metrics worsened after the implementation of the improved recommendation system. The changes in the service need to be revised, and the next testing should be conducted taking into account the calendar of marketing activities and holidays.
