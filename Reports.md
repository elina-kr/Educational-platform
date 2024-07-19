# Final Report on A/B Test of Payment Mechanism

## Introduction

The purpose of this analysis was to determine if the new payment mechanism improved the service quality on a website. An A/B test was conducted with users divided into two groups: Group A used the old payment mechanism, while Group B used the new one.

## Data Description

The dataset comprises:

- **groups.csv**: User group assignments (A – control, B – test).
- **groups_add.csv**: Additional users provided 2 days after the initial data.
- **active_studs.csv**: Users who visited the platform during the experiment.
- **checks.csv**: Details of user payments during the experiment.

## Evaluation Metrics

The following metrics were used to evaluate the payment mechanism:

1. **Conversion Rate (CR)**
2. **Average Revenue Per User (ARPU)**
3. **Average Revenue Per Paying User (ARPPU)**

## Methodology

1. **Metric Selection:** Determining relevant metrics for evaluating the new payment mechanism.
2. **Statistical Analysis:**
   - **Chi-squared test for proportions:** Comparing CR between the control and test groups.
   - **t-test for independent samples:** Comparing ARPU and ARPPU between the control and test groups.

## Results

1. **Conversion Rate:** The proportions of users who made a purchase are not significantly different between the control and test groups.
2. **User Activity:** Average user activity did not significantly differ between the control and test groups.
3. **Matches per User:** The average number of matches per user was significantly higher in the test group.

## Conclusion

Based on the analysis, the new payment mechanism led to a significant increase in ARPPU but did not significantly affect CR or ARPU. Thus, the new mechanism positively impacts revenue from paying users. It is recommended to proceed with its implementation and optimize for better conversion rates.

## Contact

For any questions or additional information, please contact me at elina8kr@gmail.com
or connect via https://www.linkedin.com/in/elina-krs/
