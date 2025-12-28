# Instagram-Reach-Analysis

A machine learning project that analyzes Instagram post reach and predicts engagement metrics based on various features including likes, saves, comments, shares, profile visits, and follows.

## Project Overview

This project performs comprehensive analysis of Instagram post performance data containing 119 posts with 13 different metrics. The analysis includes exploratory data analysis (EDA), correlation studies, data visualizations, and machine learning model development for reach prediction.

## Dataset Description

### Dataset Statistics
- **Total Posts**: 119
- **Total Features**: 13 (11 numeric, 2 text-based)
- **Missing Values**: 0 (Clean dataset)

### Features

| Feature | Type | Description |
|---------|------|-------------|
| **Impressions** | Numeric | Total number of times the post was displayed |
| **From Home** | Numeric | Impressions from follower home feeds |
| **From Hashtags** | Numeric | Impressions from hashtag discovery |
| **From Explore** | Numeric | Impressions from Instagram Explore page |
| **From Other** | Numeric | Impressions from other sources |
| **Saves** | Numeric | Number of times the post was saved |
| **Comments** | Numeric | Total number of comments on the post |
| **Shares** | Numeric | Number of times the post was shared |
| **Likes** | Numeric | Total number of likes on the post |
| **Profile Visits** | Numeric | Number of visits to the profile from this post |
| **Follows** | Numeric | Number of new followers gained from this post |
| **Caption** | Text | Post caption/description |
| **Hashtags** | Text | Hashtags used in the post |

## Key Insights from Analysis

### Impression Sources Breakdown
The analysis reveals that posts get impressions from four main sources:
- **From Home**: Impressions from follower feeds
- **From Hashtags**: Hashtag-based discovery
- **From Explore**: Instagram's algorithmic recommendations
- **Other Sources**: Additional impression sources

### Correlation Analysis Results

Top 5 factors correlated with Impressions:
1. **From Explore** (0.894) - Strongest correlation
2. **Follows** (0.889) - Strong indicator of reach
3. **Likes** (0.850) - Strong engagement metric
4. **From Home** (0.845) - Follower engagement
5. **Saves** (0.779) - Content value indicator

### Conversion Metrics
- **Profile Visit to Follow Conversion Rate**: 41.00%
  - This indicates that out of every 100 people visiting the profile from a post, approximately 41 become followers

### Engagement Relationships
Linear regression analysis shows positive correlations between:
- Impressions and Likes
- Impressions and Comments
- Impressions and Shares
- Impressions and Saves
- Profile Visits and Follows Gained

## Data Visualizations

The notebook includes multiple visualizations:
1. **Distribution plots** for impressions from different sources
2. **Word clouds** generated from post captions and hashtags
3. **Scatter plots** showing relationships between engagement metrics
4. **Pie chart** displaying impression distribution across sources
5. **Trend lines** showing linear regression relationships

## Machine Learning Model

### Model Details
- **Algorithm**: PassiveAggressiveRegressor
- **Features Used**: Likes, Saves, Comments, Shares, Profile Visits, Follows
- **Target Variable**: Impressions
- **Test Set Size**: 20%
- **Training Set Size**: 80%

### Model Performance
- **R² Score**: 0.569 (Explains 56.9% of variance in impressions)
- **Sample Prediction**: For a post with [282 Likes, 233 Saves, 4 Comments, 9 Shares, 165 Profile Visits, 54 Follows], the model predicts approximately 9,023 impressions

## Technologies Used

- **Python 3.x**
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computations
- **Matplotlib & Seaborn**: Data visualization
- **Plotly**: Interactive visualizations
- **Scikit-learn**: Machine learning model development
- **WordCloud**: Text visualization

## Files in Repository

- `Instagram data.csv` - Dataset containing Instagram post metrics
- `Instagram_Reach_Analysis.ipynb` - Jupyter notebook with complete analysis and model
- `README.md` - Project documentation (this file)

## How to Use

1. **Install Dependencies**:
   ```bash
   pip install pandas numpy matplotlib seaborn plotly scikit-learn wordcloud
   ```

2. **Run the Analysis**:
   - Open `Instagram_Reach_Analysis.ipynb` in Jupyter Notebook
   - Execute all cells to reproduce the analysis

3. **Make Predictions**:
   - Train the PassiveAggressiveRegressor model with your data
   - Use the trained model to predict impressions for new posts

## Key Takeaways

1. **Explore Page is Crucial**: The strongest correlation with impressions comes from the Explore page, suggesting algorithmic discovery is vital

2. **Engagement Drives Reach**: Likes, saves, and shares have strong correlations with total impressions

3. **Follower Conversion**: The 41% profile visit to follow conversion rate shows quality engagement

4. **Multi-metric Approach**: Using multiple engagement metrics together provides better reach prediction

5. **Content Quality Matters**: Word cloud analysis suggests data science content performs well

## Future Improvements

- Implement more advanced ML models (Random Forest, XGBoost, Neural Networks)
- Perform time-series analysis to track reach patterns over time
- Analyze caption sentiment and hashtag strategy impact
- Build a recommendation system for optimal posting times
- Create a web application for reach prediction

## Author

Sahil - Data Science Enthusiast

## License

This project is open source and available under the MIT License.

---

**Note**: This analysis is based on 119 Instagram posts and should be validated with larger datasets for more robust conclusions.
