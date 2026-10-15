# Instagram Reach and Engagement Analysis

A small-sample exploratory analysis of Instagram post impressions, reach sources, and engagement indicators.

## Project files

| File | Purpose |
|---|---|
| `Instagram data.csv` | Post-level dataset |
| `Instagram_Reach_Analysis.ipynb` | Data checks, charts, and correlation analysis |
| `README.md` | Project documentation |

## Verified dataset profile

Recalculated from the repository CSV:

| Metric | Result |
|---|---:|
| Posts/records | 119 |
| Columns | 13 |
| Missing cells | 0 |
| Total impressions | 678,775 |
| Total likes | 20,680 |
| Total saves | 18,244 |
| Total comments | 793 |
| Total shares | 1,114 |
| Total profile visits | 6,024 |
| Total follows | 2,470 |

The dataset includes impression sources (Home, Hashtags, Explore, Other), engagement counts, profile visits, follows, captions, and hashtags. These aggregates are totals across the 119 records, not account-wide long-term performance guarantees.

## Correlation results in saved notebook output

The notebook's saved correlation matrix reports:

| Numeric field | Correlation with impressions |
|---|---:|
| From Explore | 0.894 |
| Follows | 0.889 |
| Likes | 0.850 |
| From Home | 0.845 |
| Saves | 0.779 |
| Profile Visits | 0.761 |
| Shares | 0.635 |
| From Other | 0.593 |
| From Hashtags | 0.561 |
| Comments | −0.029 |

These are Pearson correlations in a 119-row dataset. Correlation does not establish causation. Some reach-source fields may contribute mathematically to total impressions, so their correlation with impressions should not be interpreted as independent causal impact.

## Workflow

1. Load `Instagram data.csv` in the notebook.
2. Inspect schema, missing values, and numeric distributions.
3. Compare impression sources and engagement totals.
4. Explore correlations and scatterplots.
5. Interpret the results with sample-size and feature-definition caveats.

## Technology

Python, pandas, NumPy, Jupyter Notebook, and Plotly/visualization tools imported by the notebook.

## Reproduce

Open `Instagram_Reach_Analysis.ipynb` in Jupyter or Colab and run it from top to bottom. Install the libraries imported by the notebook; a root-level `requirements.txt` was not present in the repository inventory.

## Limitations

- The dataset contains only 119 posts; results may not generalize to other accounts or time periods.
- Caption and hashtag data may be subject to platform and data-source reuse restrictions.
- Reach-source counts may not be mutually exclusive or exhaustive; do not assume they sum to total impressions.
- Descriptive correlations do not prove that one engagement activity causes another.

## Skills demonstrated

Data profiling, EDA, descriptive statistics, correlation analysis, visualization, and cautious interpretation of small datasets.

## Author

Sahil Gaikwad · [GitHub](https://github.com/sahil2003-ai) · [LinkedIn](https://www.linkedin.com/in/sahil-gaikwad-a76b7224a/)
