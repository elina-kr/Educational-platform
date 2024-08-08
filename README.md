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
## The following metrics are used to evaluate the new payment mechanism:

### Conversion Rate (CR)

**Formula:**
CR = (Number of users who made a purchase / Total number of active users) × 100

### Average Revenue Per User (ARPU)

**Formula:**
ARPU = Total Revenue / Total number of active users

### Average Revenue Per Paying User (ARPPU)

**Formula:**
ARPPU = Total revenue from paying users / Number of paying users


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

# SQL Queries for Educational Platform Analysis

## Overview

This project focuses on analyzing data from an educational platform to assess student performance and the effectiveness of a new payment mechanism. Two SQL tasks were undertaken:

1. **Identifying Diligent Students**: An SQL query was written to determine the number of diligent students who correctly solved at least 20 problems in the current month.
2. **Optimizing Funnel Conversion**: A complex SQL query was developed to analyze user behavior and payment conversions, comparing metrics between control and experimental groups.

## Goals

1. **Diligent Student Identification**: 
   - To write an efficient SQL query that identifies students who demonstrate high diligence by correctly solving a significant number of problems in a given month.
  
2. **Funnel Conversion Optimization**:
   - To evaluate the impact of a new payment screen on various key performance indicators (KPIs) such as ARPU, ARPAU, and conversion rates for different user segments.

## Data Description

### Tables Used:

1. **default.peas**:
   - **st_id** (int): Student ID.
   - **timest** (timestamp): Time when a problem was solved.
   - **correct** (bool): Whether the problem was solved correctly.
   - **subject** (text): The subject area of the problem.

2. **default.studs**:
   - **st_id** (int): Student ID.
   - **test_grp** (text): Group assignment (control or pilot) for the experiment.

3. **default.final_project_check**:
   - **st_id** (int): Student ID.
   - **sale_time** (timestamp): Time of purchase.
   - **money** (int): Amount paid.
   - **subject** (text): Subject for which the course was purchased.

## Metrics

### 1. Diligent Student Identification

**Metric**: Number of students who correctly solved at least 20 problems in the current month.

### 2. Funnel Conversion Optimization

The following metrics were calculated for each user group:

- **ARPU**: Average Revenue Per User.
- **ARPAU**: Average Revenue Per Active User.
- **CR (Conversion Rate)**: The proportion of users who made a purchase.
- **CR_activ**: Conversion rate of active users to paying users.
- **CR_math**: Conversion rate of users active in mathematics to purchasing a mathematics course.

## Results

### 1. Diligent Student Identification

The SQL query identified **136 diligent students** who solved at least 20 problems correctly in the current month.

### 2. Funnel Conversion Optimization

The SQL query yielded the following results:

| Group   | ARPU    | ARPAU   | CR    | CR_activ | CR_math |
|---------|---------|---------|-------|----------|---------|
| Control | 4540.98 | 10820.31| 0.05  | 0.12     | 0.18    |
| Pilot   | 11508.47| 35000.00| 0.11  | 0.34     | 0.40    |

**Key Findings**:
- The pilot group had a significantly higher ARPU, ARPAU, and conversion rates across all metrics compared to the control group.
- The new payment screen in the pilot group led to better overall performance, indicating its effectiveness in converting users to paying customers, especially in the mathematics discipline.

## Conclusion

1. **Diligent Student Identification**: The query effectively identified diligent students, which can be used for further targeted interventions to enhance their learning experience.

2. **Funnel Conversion Optimization**: The new payment screen was highly effective, significantly improving user engagement and revenue metrics. It is recommended to implement the new payment screen platform-wide, with a focus on further optimizing the user journey for mathematics courses.

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
