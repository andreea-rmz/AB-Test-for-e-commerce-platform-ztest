# A/B Test for an e-commerce platform 

(Sprint 10, focus on test, not experiment; treatment unknown)

This project analyzes an A/B test conducted by an e-commerce platform to evaluate whether Group B performs better than Group A across critical business metrics. The workflow includes data preprocessing, cumulative metric construction (revenue, orders, conversion rate, AOV), and time-series visualization to observe performance trends throughout the experiment. Outliers were detected using the 95th and 99th percentiles for both order value and user purchase frequency, and filtered datasets were re-evaluated to ensure the robustness of conclusions.
Statistical significance was assessed using the non-parametric Mann-Whitney U test on both raw and cleaned data. The results show a significant improvement in conversion for Group B, with p = 0.017 on raw data (+13.8% relative gain) and p = 0.020 after filtering anomalies (+15.8%). Differences in AOV were not statistically significant after removing outliers (p = 0.939), indicating that the initial 25% increase in Group B’s average order value was driven by extreme values rather than a true effect.
Overall, the cumulative revenue curves, conversion trajectories, and statistical tests consistently demonstrate that Group B outperforms Group A in driving conversions.
Recommended decision: stop the experiment and adopt Group B as the winning variant.
