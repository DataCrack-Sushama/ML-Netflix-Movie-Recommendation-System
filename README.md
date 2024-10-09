# Case-Study-ML-Netflix-Movie-Recommendation-System

A Machine Learning Case Study for a movie recommendation system using collaborative filtering and content-based filtering.

## Business Problem

Netflix connects users to movies they love by recommending films based on their viewing history. Their recommendation system, **CinematchSM**, predicts whether a user will enjoy a movie based on their ratings of other movies. Netflix continuously looks for ways to improve its recommendation accuracy to enhance customer satisfaction and business performance.

This case study aims to explore alternative machine learning approaches that could improve Cinematch's accuracy by at least 10%. The goal is to predict user ratings more accurately, which would allow Netflix to make better recommendations.

Credits: [Netflix Prize Rules](https://www.netflixprize.com/rules.html)

## Problem Statement

Netflix provided anonymous rating data and set a challenge to beat the accuracy of their Cinematch algorithm by at least 10% on the same dataset. The task is to predict user ratings of movies that they haven't watched, minimizing the error between predicted and actual ratings.

## Data Sources

- [Netflix Prize Dataset](https://www.kaggle.com/netflix-inc/netflix-prize-data)
- [Netflix Blog: Recommendations Beyond the 5 Stars](https://medium.com/netflix-techblog/netflix-recommendations-beyond-the-5-stars-part-1-55838468f429)
- [Surprise Library](http://surpriselib.com/)
- [Research Paper on Matrix Factorization](http://courses.ischool.berkeley.edu/i290-dm/s11/SECURE/a1-koren.pdf)
- [SVD Decomposition Video](https://www.youtube.com/watch?v=P5mlg91as1c)

## Objectives and Constraints

### Objectives:
- Predict the rating a user would give to a movie they haven't rated yet.
- Minimize the difference between predicted and actual ratings, using metrics such as RMSE (Root Mean Square Error) and MAPE (Mean Absolute Percentage Error).

### Constraints:
- Some level of interpretability in the results.
- Low latency is not a critical requirement since recommendations can be precomputed.

## Data Overview

- **Unique Movie IDs**: 17,770
- **Unique User IDs**: 480,189
- **Ratings**: 1 to 5 stars, on an integer scale.
- **Timestamp**: When the user rated the movie (YYYY-MM-DD format).

## Getting Started

To run the project, download or clone the repository and open the `NetflixMoviesRecommendation.ipynb` file using Jupyter or any compatible notebook environment.

## Prerequisites

Before running the project, ensure the following tools and libraries are installed:

- Python 3
- [Anaconda](https://www.anaconda.com/download/): Includes Jupyter Notebook and most required libraries like Pandas, Seaborn, Matplotlib, and Scikit-learn.
- XGBoost
- Surprise (for recommendation models)

### Installation Steps

1. **Python 3**: [Download Python](https://www.python.org/downloads/)
2. **Anaconda**: [Download Anaconda](https://www.anaconda.com/download/)
3. **XGBoost**: Install using Conda:
   ```bash
   conda install -c conda-forge xgboost
4.Surprise: Install using pip: pip install surprise

Project Structure
NetflixMoviesRecommendation.ipynb: The main notebook containing data preprocessing, model building, and predictions.
data/: Contains the Netflix Prize dataset.
README.md: Project documentation.

Built With
Jupyter Notebook: Used for interactive coding and documentation.
Scikit-learn: Machine learning algorithms and evaluation metrics.
Surprise: Specialized library for building and evaluating recommendation systems.
XGBoost: Used for regression models.
Pandas: For data manipulation and analysis.
NumPy: For numerical operations.
Seaborn & Matplotlib: For data visualization.

Acknowledgments
This project is inspired by the Applied AI Course and research from various papers, blogs, and libraries mentioned above.
