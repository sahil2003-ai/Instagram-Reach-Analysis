# Instagram Reach and Engagement Analysis

> Small-data analysis of Instagram post reach, impressions, and engagement indicators.

![Status](https://img.shields.io/badge/Status-Portfolio--Project-blue)

## 📌 Table of Contents

- [Overview](#overview)
- [Problem Statement](#problem-statement)
- [Objectives](#objectives)
- [Features](#features)
- [Dataset](#dataset)
- [Tech Stack](#tech-stack)
- [Project Workflow](#project-workflow)
- [Repository Structure](#repository-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Results and Insights](#results-and-insights)
- [Screenshots](#screenshots)
- [Challenges and Solutions](#challenges-and-solutions)
- [Limitations](#limitations)
- [Future Improvements](#future-improvements)
- [What I Learned](#what-i-learned)
- [Author](#author)
- [License](#license)

## 📖 Overview

Small-data analysis of Instagram post reach, impressions, and engagement indicators. This README documents the intended workflow and the files available in the repository. Verify all outputs against the current code and data before using them as evidence.

## 🎯 Problem Statement

Creators need to understand how reach and engagement metrics vary across posts, while avoiding overinterpretation of small samples.

## 🎯 Objectives

- Inspect and clean post-level data.
- Explore distributions and relationships between metrics.
- Evaluate any prediction task without target leakage.

## ✨ Features

- Instagram data.csv dataset.
- Notebook-based EDA.
- Reach and engagement analysis.

## 📂 Dataset

The repository CSV contains **119 rows × 13 columns**.

- **Fields include:** impressions, reach sources (home, hashtags, explore, other), saves, comments, shares, likes, profile visits, follows, caption, and hashtags.
- **Target variable:** No single target is assumed; define it explicitly if modelling.
- Check missing values and duplicates in the notebook. Document the source, collection period, and any restrictions on reusing captions or hashtags.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python/pandas | Data handling |
| Jupyter Notebook | Analysis |
| Visualization libraries | Charts as implemented |

## 🔄 Project Workflow

1. Load Instagram data.csv in Instagram_Reach_Analysis.ipynb.
2. Inspect row/column counts, data types, missing values, and duplicates.
3. Verify definitions for impressions, reach sources, likes, comments, saves, shares, visits, and follows.
4. Use descriptive statistics and visualizations to inspect distributions.
5. Explore relationships between reach sources and engagement indicators.
6. If modelling is used, define the target and remove features that directly encode it.
7. Use a holdout split and baseline, then document findings with caveats.

## 🗂️ Repository Structure

```text
Instagram-Reach-Analysis/
├── Instagram data.csv
├── Instagram_Reach_Analysis.ipynb
└── README.md
└── README.md
```

The list above highlights known project files and folders; inspect the repository for the complete current structure.

## ⚙️ Installation

### Prerequisites

- Install the tools listed in the Tech Stack that apply to this project.
- For Python projects, use a Python version compatible with the dependencies actually imported by the code.
- For Power BI projects, use Power BI Desktop.

### Setup

Open the notebook in Jupyter or Colab and install the packages imported by the notebook. A requirements.txt was not listed at the repository root.

Do not run generic commands that do not match the files in this repository. Confirm the data paths, database dialect, and package versions before execution.

## ▶️ Usage

Run Instagram_Reach_Analysis.ipynb from top to bottom after checking the CSV path.

## 📊 Results and Insights

### Verified dataset dimensions

| Check | Result |
|---|---:|
| Rows | 119 |
| Columns | 13 |

The saved notebook provides exploratory analysis, but numerical correlations, leading reach sources, and model metrics were not independently reproduced in this review. Add findings only with supporting calculations or charts. Correlation should not be interpreted as causation.

## 🖼️ Screenshots

No image files were confirmed for this repository during this update. If you have screenshots, upload them into an `images/` folder, then embed each real path here with a short caption. Do not use placeholder image paths.

## 🧩 Challenges and Solutions

| Challenge | Solution / validation approach |
|---|---|
| Potential target leakage | Reach-source fields may directly contribute to total impressions; check target definitions before modelling. |

## ⚠️ Limitations

- The sample is small (119 posts) and may not generalize to other accounts or time periods.
- Reach-source fields may overlap mathematically with impressions; check target definitions for leakage before modelling.
- Document the data source, collection window, and any restrictions on caption/hashtag reuse.

## 🚀 Future Improvements

- [ ] Add charts under images/.
- [ ] Document data provenance and feature definitions.
- [ ] If predicting, report holdout metrics and leakage checks.

## 📚 What I Learned

- EDA and correlation analysis.
- Careful feature selection for small datasets.

## 👤 Author

**Sahil Gaikwad**

- GitHub: [sahil2003-ai](https://github.com/sahil2003-ai)
- LinkedIn: [Sahil Gaikwad](https://www.linkedin.com/in/sahil-gaikwad-a76b7224a/)

## 📄 License

Check data rights and repository license.
