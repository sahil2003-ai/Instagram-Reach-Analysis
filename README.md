# Instagram Reach and Engagement Analysis

An exploratory data analysis project examining Instagram post impressions, reach sources, and engagement indicators across a post-level dataset.

![Python](https://img.shields.io/badge/Python-EDA-blue) ![Pandas](https://img.shields.io/badge/Pandas-Analysis-150458)

## Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Workflow](#workflow)
- [Results and Metrics](#results-and-metrics)
- [Technology Stack](#technology-stack)
- [Repository Structure](#repository-structure)
- [Run the Notebook](#run-the-notebook)
- [Limitations and Next Steps](#limitations-and-next-steps)

## Overview
The notebook analyzes impressions, engagement actions, profile visits, follows, and reach-source patterns. The aim is to describe the dataset and generate hypotheses for future content experiments.

## Dataset
Source file: `Instagram data.csv`.

| Metric | Verified value |
|---|---:|
| Rows/posts | 119 |
| Columns | 13 |
| Missing cells | 0 |
| Total impressions | 678,775 |
| Total likes | 20,680 |
| Total saves | 18,244 |
| Total comments | 793 |
| Total shares | 1,114 |
| Total profile visits | 6,024 |
| Total follows | 2,470 |

The data includes impressions by source (Home, Hashtags, Explore, Other), engagement counts, profile visits, follows, captions, and hashtags. Check source and reuse terms before redistributing caption or hashtag text.

## Workflow
1. Load `Instagram data.csv`.
2. Inspect dimensions, types, missing values, and numeric distributions.
3. Calculate totals and post-level engagement summaries.
4. Generate descriptive plots and a Pearson correlation matrix.
5. Interpret correlations in light of sample size and feature definitions.
6. Form hypotheses for controlled follow-up tests rather than claiming causation.

## Results and Metrics
The 119 records contain 678,775 impressions, 20,680 likes, 18,244 saves, 793 comments, 1,114 shares, 6,024 profile visits, and 2,470 follows.

Saved notebook correlations with impressions include:

| Field | Pearson correlation |
|---|---:|
| From Explore | 0.894 |
| Follows | 0.889 |
| Likes | 0.850 |
| From Home | 0.845 |

These are associations in this dataset, not proof that increasing a specific metric will cause more impressions. Small sample size and the relationships between reach and engagement variables should be considered.

## Technology Stack
- Python
- pandas and NumPy
- Jupyter Notebook
- Visualization libraries used by the notebook

## Repository Structure
```text
Instagram-Reach-Analysis/
├── Instagram data.csv
├── Instagram_Reach_Analysis.ipynb
└── README.md
```

## Run the Notebook
```bash
git clone https://github.com/sahil2003-ai/Instagram-Reach-Analysis.git
cd Instagram-Reach-Analysis
python -m venv .venv
```
Activate the environment, install pandas, NumPy, and the notebook's plotting dependencies, then open `Instagram_Reach_Analysis.ipynb` in Jupyter or Colab.

## Limitations and Next Steps
- Document the dataset source and license.
- Add engagement-rate definitions with explicit denominators.
- Test content hypotheses using a larger dataset and controlled comparisons.
- Add genuine charts/screenshots if stored in the repository.
- Avoid interpreting correlation as causal impact.

## Skills Demonstrated
Data cleaning, descriptive statistics, correlation analysis, visualization, and social-media performance interpretation.

## Author
**Sahil Gaikwad** · [GitHub](https://github.com/sahil2003-ai) · [LinkedIn](https://www.linkedin.com/in/sahil-gaikwad-a76b7224a/)
