# Educational-platform

# A/B Testing of New Payment Mechanism

## Overview

This project involves analyzing an A/B test conducted to evaluate the effectiveness of a new payment mechanism on a website. The goal is to determine whether the new payment mechanism should be implemented for all users. Users were divided into two groups: Group A (control) continued using the old payment mechanism, while Group B (test) used the new payment mechanism.

## Goals

1. Identify key metrics to assess the impact of the new payment mechanism.
2. Statistically compare these metrics between the control and test groups to determine if the new mechanism offers significant improvements.

## Data Description

The dataset includes the following CSV files:

- **groups.csv**: Contains information about user group assignments (A – control, B – test).
- **groups_add.csv**: An additional file with users added 2 days after the initial data transfer.
- **active_studs.csv**: Information about users who visited the platform during the experiment.
- **checks.csv**: Details of user payments during the experiment.

## Metrics for Evaluation

The following metrics are used to evaluate the new payment mechanism:

1. **Conversion Rate (CR)**
   - Formula: \( \text{CR} = \left(\frac{\text{Number of users who made a purchase}}{\text{Total number of active users}}\right) \times 100 \)

2. **Average Revenue Per User (ARPU)**
   - Formula: \( \text{ARPU} = \frac{\text{Total Revenue}}{\text{Total number of active users}} \)

3. **Average Revenue Per Paying User (ARPPU)**
   - Formula: \( \text{ARPPU} = \frac{\text{Total revenue from paying users}}{\text{Number of paying users}} \)

## Methodology

1. **Metric Selection:** Identifying relevant metrics for assessing the impact of the new payment mechanism.
2. **Statistical Analysis:**
   - **Chi-squared test for proportions:** To compare conversion rates between groups.
   - **t-test for independent samples:** To compare ARPU and ARPPU between groups.

## Results

1. **Conversion Rate:** No significant change between the control and test groups.
2. **ARPU:** No significant increase between the control and test groups.
3. **ARPPU:** Significant increase in the test group compared to the control group.

## Conclusion

The new payment mechanism led to a significant increase in ARPPU, suggesting that while conversion rates and ARPU did not improve, the new mechanism positively impacted revenue from paying users. It is recommended to continue using the new payment mechanism with potential optimizations to increase conversion rates.

## Contact

For any questions or additional information, please contact me at elina8kr@gmail.com.
My LinkedIn: [https://www.linkedin.com/in/elina-krs/](https://www.linkedin.com/in/elina-krs/)

## Key Skills

- Python
- Pandas
- NumPy
- Seaborn
- SciPy
- Statistics
- A/B Testing
- Data Analysis

## Repository Contents

- **Educational-platform:** Jupyter notebooks with detailed analysis.
- **reports:** Final analytical report.
