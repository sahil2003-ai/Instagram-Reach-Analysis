# Instagram Reach and Engagement Analysis

A small-data analytics project exploring Instagram post reach and its relationship with engagement metrics.

## Dataset
The existing README describes 119 posts and 13 fields, including impressions, reach sources, likes, saves, comments, shares, profile visits, follows, captions, and hashtags. Verify these details against the actual data file.

## Objectives
- Explore where impressions originate.
- Examine relationships between reach and engagement.
- Visualize patterns across posts.
- Experiment with predicting reach from available features.

## Analysis Areas
- Descriptive statistics and missing-value checks
- Correlation analysis
- Engagement and conversion metrics
- Visual comparisons across reach sources
- Regression modelling, if implemented in the notebook

## Tools
Python, pandas, visualization libraries, and scikit-learn where used.

## Important Modelling Consideration
Features such as impressions-from-home, impressions-from-explore, and other impression sources may sum to or directly determine total impressions. Using them to predict total impressions can create target leakage or a near-mechanical relationship. Clearly separate explanatory analysis from a genuine forecasting task and use a valid holdout strategy.

## Skills Demonstrated
EDA, correlation analysis, feature interpretation, visualization, and small-data modelling.

## Recommended Improvements
- Document the data source and collection period.
- Include a data dictionary and metric definitions.
- Report only verified findings.
- Add a baseline and held-out evaluation metrics if prediction is included.
- Explain the small sample size and limits on generalization.

> Correlation does not establish causation, and results from a small sample may not generalize to other accounts or time periods.