# Instagram Reach and Engagement Analysis

A small-data project exploring Instagram post impressions, reach sources, and engagement indicators.

## Step-by-step workflow

1. Load `Instagram data.csv` in `Instagram_Reach_Analysis.ipynb`.
2. Inspect the number of rows, column types, missing values, and duplicates.
3. Clean column names and verify how impressions, reach sources, likes, comments, saves, shares, visits, and follows are defined.
4. Use descriptive statistics and visualizations to understand distributions and outliers.
5. Examine relationships between reach sources and engagement metrics.
6. If training a prediction model, define the target and remove features that directly calculate or leak the target.
7. Split data appropriately, compare with a baseline, and evaluate on held-out observations.
8. Summarize findings without claiming that correlation proves causation.

## Tools
Python, pandas, Jupyter Notebook, visualization and ML libraries where used.

## Dataset
The existing README describes 119 posts and 13 fields; verify these values against the CSV before quoting them.

## Screenshots
No image files were found in the repository root. Add selected charts under `images/` and embed them here.

## Limitations
The sample is small and may not generalize to other accounts or time periods. Reach-source features can leak the target if used carelessly.

## Next improvements
Document data source and collection period, add charts, explain feature selection, and report verified metrics.