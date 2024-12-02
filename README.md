# Sleep Health and Lifestyle Analysis
Group - 9
Laasya Priya Vemuri - A20561469
Arundathi Nalla - A20549875
Swathi Yadlapalli - A20545355
Dinesh Datta Molli - A20548385

This repository contains a Python-based machine learning pipeline to analyze sleep health and lifestyle data. The pipeline includes data preprocessing, visualization, dimensionality reduction, clustering, classification, and model evaluation techniques.


## Table of Contents

- [Dataset Overview](#dataset-overview)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Results](#results)
- [License](#license)


## Dataset Overview

The dataset, `Sleep_health_and_lifestyle.csv`, contains the following key features:

- **Demographic Information:** Gender, Age, Occupation.
- **Health Metrics:** Sleep Duration, Quality of Sleep, BMI Category, Blood Pressure, Heart Rate, etc.
- **Target Variable:** `Sleep Disorder` (e.g., Sleep Apnea, Insomnia).


## Requirements

The project uses the following Python libraries:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `sklearn`
- `imblearn`
- `umap-learn`

Install the required packages using the following command:

```bash
pip install -r requirements.txt
```

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your_username/sleep-health-analysis.git
   cd sleep-health-analysis
   ```

2. Place the dataset file `Sleep_health_and_lifestyle.csv` in the root directory of the repository.

3. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

Run the Python script to execute the pipeline:

```bash
python sleep_health_analysis.py
```

### Features of the Script:

1. **Data Exploration:**
   - Overview of dataset, missing value analysis, and target distribution visualization.
   
2. **Preprocessing:**
   - Encoding categorical variables.
   - Scaling numerical data.
   - Handling class imbalance using SMOTE.

3. **Visualization:**
   - Correlation heatmap.
   - Dimensionality reduction with PCA, t-SNE, and UMAP.
   - Target distribution and clustering visualization.

4. **Feature Engineering:**
   - Recursive Feature Elimination (RFE) for feature selection.

5. **Model Training and Evaluation:**
   - Random Forest Classifier with hyperparameter tuning.
   - Gradient Boosting Classifier.
   - Cross-validation and performance metrics (accuracy, precision, recall, F1-score).


## Features

### Dimensionality Reduction
- Implemented PCA, t-SNE, and UMAP to project high-dimensional data into 2D for visualization.

### Clustering
- K-means clustering to explore potential groupings within the data.
- Evaluated using silhouette score.

### Classification
- Random Forest and Gradient Boosting models for prediction of sleep disorders.
- Hyperparameter tuning with `GridSearchCV`.

### Visualization
- Comprehensive visualizations for insights and model interpretation, including feature importance.

## Results

- **Best Model:** Random Forest with hyperparameter tuning.
- **Accuracy:** 95.45%
- **Feature Importance:**
  Key predictors include Sleep Duration, Physical Activity Level, Stress Level, BMI Category, and Daily Steps.
