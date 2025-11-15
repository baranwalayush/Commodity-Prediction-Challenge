#### SoE JNU EN502 Monsoon 2025 Machine Learning Project

# Commodity-Prediction-Challenge
## Project Summary: Approach & Solution Workflow

### Data Loading
- Implemented an automatic loader that detects whether the notebook is running on Kaggle or locally and loads the dataset accordingly.

### Exploratory Data Analysis
- Performed targeted EDA including exchange-group distributions, pair-level target analysis, time-series inspection of selected assets, and spread visualizations across multiple target pairs.

### Competition Metric
- Implemented the custom RankCorr-Sharpe evaluation function as required by the competition.

### Dataset Preparation
- Applied preprocessing, feature engineering (lags, rolling statistics, etc.), and created train–test splits for modeling.

### Model Development
- Trained four models:

    - RandomForest Regressor

    - CatBoost Regressor

    - Single multi-output LightGBM

    - Multiple single-output LightGBM models

### Model Training & Evaluation
- The RandomForest baseline achieved:
    - TRAIN RankCorr-Sharpe: 6.8863
    - TEST RankCorr-Sharpe: 1.9417
- Additional cross-validation was performed using the single-output LightGBM models.

### Prediction Pipeline
- Implemented the final predict() function for seamless Kaggle inference.

### Conclusion
- Although the model performance was modest, the project provided strong learning on financial time-series modeling, custom metrics, and multi-output ML pipelines. Future improvements will continue refining features and model architectures.
