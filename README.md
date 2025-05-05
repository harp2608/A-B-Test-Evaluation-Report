A/B Test Evaluation Report
Part 1: Data Preparation
We loaded and merged five datasets (users, homepage, searchpage, paypage, and payconf) based on user_id. Then,
we randomly assigned users into Control and Test groups using a binomial distribution with p = 0.495. To track
conversion, we created a binary column 'converted' where users who reached the paypage were considered converted.


Part 2: Exploratory Data Analysis
Conversion rate for each group was calculated and visualized. Device-wise differences were also explored, indicating
potential confounding variables.


Part 3: Statistical Hypothesis Testing
Null Hypothesis (H0): Conversion rates are equal between Control and Test. Alternative Hypothesis (H1): Test group
has a higher conversion rate. Using a one-tailed z-test, we found p-value = 0.2814. Since p > 0.05, we fail to reject the
null hypothesis.


Part 4: Interpretation and Discussion
The difference in conversion rates is not statistically significant. Limitations include sample size, device mix imbalance,
and potential external factors. Future analysis may include longer test duration, user segmentation, or Bayesian
analysis.


Part 5: Recommendation
Do not switch to the treatment paywall yet. Gather more data to reach statistical significance and explore other
influencing factors.
