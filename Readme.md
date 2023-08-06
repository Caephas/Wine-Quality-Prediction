# Wine Quality Prediction - README

## Overview
This script aims to predict the quality of red wine based on several input features. Instead of using the actual quality ratings, the model is trained to predict if a wine is of "good" or "bad" quality.

## Table of Contents
1. [Dependencies](#dependencies)
2. [Data Collection and Analysis](#data-collection-and-analysis)
3. [Data Preprocessing](#data-preprocessing)
4. [Model Training and Evaluation](#model-training-and-evaluation)
5. [Building a Predictive System](#building-a-predictive-system)

## Dependencies
* numpy
* pandas
* matplotlib
* seaborn
* sklearn

To install all dependencies, you can use:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

## Data Collection and Analysis
1. **Loading Data**:
   - The dataset is loaded into a pandas DataFrame from a CSV file named 'winequality-red.csv'.

2. **Exploratory Data Analysis**:
   - Basic statistical properties of the dataset are calculated.
   - The distribution of wine quality scores in the dataset is visualized using seaborn's `catplot`.
   - The relationship between different features and wine quality is visualized using bar plots.

3. **Correlation Analysis**:
   - A heatmap is used to visually understand the correlation between various features of the dataset.

## Data Preprocessing
1. **Feature Separation**:
   - The dataset is divided into features (`X`) and target labels (`Y`).

2. **Label Binarization**:
   - Wine quality scores are binarized into two categories:
     - `1` for good quality (wine quality >= 7)
     - `0` for bad quality (wine quality < 7).

3. **Data Splitting**:
   - The dataset is divided into a training set (80% of data) and a test set (20% of data).

## Model Training and Evaluation
1. **Random Forest Classifier**:
   - A RandomForestClassifier is chosen for training. This ensemble method constructs multiple decision trees during training.

2. **Model Evaluation**:
   - The trained model's performance is evaluated on the test set. The accuracy score, which indicates the ratio of correctly predicted samples to the total samples, is calculated.

## Building a Predictive System
- An example of how to use the trained model to predict wine quality is provided. Given the feature values of a wine sample, the system can predict whether the wine is of "good" or "bad" quality.

## Conclusion
This script showcases the end-to-end process of building a binary classification system using a RandomForestClassifier and the wine quality dataset. With a suitable dataset, this approach can be a helpful starting point for more complex predictive models in wine quality assessment or similar tasks in different domains.