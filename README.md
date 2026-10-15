# Instagram Reach and Engagement Analysis

> An exploratory data analysis project examining Instagram post impressions, reach sources, and engagement indicators across a small post-level dataset.

![Python](https://img.shields.io/badge/Python-EDA-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458)
![Status](https://img.shields.io/badge/Status-Exploratory-yellow)

## 📌 Table of Contents

- [Overview](#-overview)
- [Problem Statement](#-problem-statement)
- [Objectives](#-objectives)
- [Features](#-features)
- [Dataset](#-dataset)
- [Tech Stack](#-tech-stack)
- [Project Workflow](#-project-workflow)
- [Repository Structure](#-repository-structure)
- [Installation](#-installation)
- [Usage](#-usage)
- [Results and Insights](#-results-and-insights)
- [Screenshots](#-screenshots)
- [Challenges and Solutions](#-challenges-and-solutions)
- [Limitations](#-limitations)
- [Future Improvements](#-future-improvements)
- [What I Learned](#-what-i-learned)
- [Author](#-author)
- [License](#-license)

## 📖 Overview

This project analyzes post-level Instagram metrics to explore impressions, engagement actions, profile visits, follows, and reach-source patterns. It uses Python data analysis and visualizations to turn raw post metrics into descriptive insights.

## 🎯 Problem Statement

Creators and social media analysts need to understand how reach and engagement vary across posts. Descriptive analysis can reveal patterns worth testing, but it must account for small samples and avoid claiming that correlated metrics cause one another.

## 🎯 Objectives

- Profile the dataset and validate data completeness.
- Summarize reach and engagement totals.
- Compare impressions with numeric engagement and reach-source fields.
- Identify hypotheses for future content experiments.

## ✨ Features

- Data-quality checks and numeric summaries.
- Aggregate totals for impressions, likes, saves, comments, shares, profile visits, and follows.
- Pearson correlation analysis with impressions.
- Charts for exploring post-level distributions and relationships.

## 📂 Dataset

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

The data includes impressions by source (Home, Hashtags, Explore, Other), engagement counts, profile visits, follows, captions, and hashtags. Dataset source and reuse terms should be checked before redistributing captions or hashtag text.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Analysis |
| pandas / NumPy | Data manipulation and numeric summaries |
| Jupyter Notebook | Reproducible workflow |
| Visualization libraries imported in the notebook | Charts and exploratory plots |

## 🔄 Project Workflow

1. Load `Instagram data.csv`.
2. Inspect dimensions, data types, missing values, and numeric distributions.
3. Calculate engagement and impressions totals.
4. Generate descriptive charts and a correlation matrix.
5. Interpret correlations in light of sample size and feature definitions.
6. Identify follow-up hypotheses rather than claiming causal effects.

## 🗂️ Repository Structure

```text
Instagram-Reach-Analysis/
├── Instagram data.csv
├── Instagram_Reach_Analysis.ipynb
└── README.md
```

## ⚙️ Installation

### Prerequisites

- Python
- Jupyter Notebook or Google Colab
- Git

### Setup

```bash
git clone https://github.com/sahil2003-ai/Instagram-Reach-Analysis.git
cd Instagram-Reach-Analysis
python -m venv .venv
```

Activate the environment and install pandas, NumPy, and the visualization libraries imported by the notebook. A root-level `requirements.txt` was not found in the reviewed inventory.

## ▶️ Usage

Open `Instagram_Reach_Analysis.ipynb` in Jupyter or Colab and run the cells from top to bottom with `Instagram data.csv` at the expected path.

## 📊 Results and Insights

### Key Findings

The CSV contains 119 records and no missing cells. Across those records there are 678,775 impressions, 20,680 likes, 18,244 saves, 793 comments, 1,114 shares, 6,024 profile visits, and 2,470 follows.

The saved notebook correlation matrix reports the following Pearson correlations with impressions:

| Field | Correlation |
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

Some reach-source metrics may be mathematically related to total impressions, so these correlations are not evidence of independent causal impact.

### Evaluation

These are descriptive summaries, not a predictive model evaluation. The sample is limited to 119 posts and may not generalize to other accounts or periods.

## 🖼️ Screenshots

No verified screenshot path was confirmed during the repository audit. Add actual notebook charts exported from this analysis rather than using mock visuals.

## 🧩 Challenges and Solutions

| Challenge | Approach |
|---|---|
| Reach sources may overlap with total impressions | Document field definitions before interpreting correlation |
| Small sample size | Treat results as exploratory and validate hypotheses on more posts |
| Correlation can be misread as causation | Frame results as associations and propose controlled content tests |

## ⚠️ Limitations

- Only 119 post records are included.
- Data provenance and license are not documented in the repository.
- Reach-source counts may not be mutually exclusive or sum to total impressions.
- Correlation does not establish causation or predict future reach.

## 🚀 Future Improvements

- [ ] Add dataset source and data dictionary.
- [ ] Create a reusable engagement-rate definition with explicit denominator.
- [ ] Compare content types and posting periods if the data supports it.
- [ ] Validate hypotheses on a larger, time-separated sample.

## 📚 What I Learned

- Profiling small social-media datasets.
- Summarizing engagement and reach indicators.
- Using correlation matrices without overstating causal meaning.
- Turning exploratory patterns into testable content hypotheses.

## 👤 Author

**Sahil Gaikwad**

- GitHub: [sahil2003-ai](https://github.com/sahil2003-ai)
- LinkedIn: [Sahil Gaikwad](https://www.linkedin.com/in/sahil-gaikwad-a76b7224a/)

## 📄 License

Confirm the repository license and source dataset reuse terms before redistribution.
