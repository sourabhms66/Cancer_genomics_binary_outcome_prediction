# Project Overview: Cancer Genomics Binary Outcome Prediction
This project focuses on predicting binary outcomes in cancer genomics data using various machine learning classifiers. The dataset is used select certain features from genomics data, which have been cleaned, analyzed, and utilized to build different models for classification. Below is a step-by-step explanation of the workflow and methods used in the project.

## 1. Data Loading and Exploration
We begin by loading the dataset into a pandas DataFrame. The data is inspected for missing values and class distribution.

   *Missing Values:* A check is performed to ensure the dataset has no missing values.
   
   *Class Distribution:* A bar plot of class counts is generated to visually inspect the balance of the dataset.

## 2. PCA Analysis
Principal Component Analysis (PCA) is applied to reduce the dimensionality of the dataset, which helps visualize the class separation in a 2D space.

 *PCA Transformation:* The data is reduced to two principal components.
 
 *Visualization:* A scatter plot is generated to show the separation between classes.

## 3. Feature Importance Analysis
Three different methods are used to identify important features:

 *Random Forest Classifier:* Feature importances are extracted based on a trained Random Forest model.
 
 *ANOVA F-statistic:* SelectKBest is used to identify the top features using the F-statistic.
 
 *Relief-based Algorithm:* The ReliefF method selects features based on their relevance to the target class.

 ## 4. Model Building and Evaluation
Several machine learning classifiers are used to predict the binary outcome:

#### Logistic Regression
#### Decision Tree Classifier
#### Random Forest Classifier
#### Support Vector Machine (SVC)
#### K-Nearest Neighbors (KNN)

## Each classifier is trained on 80% of the data and evaluated on the remaining 20%. Key evaluation metrics include:

#### Accuracy
#### Precision
#### Recall
#### F1-Score

## 5. Confusion Matrix and Metric Visualization
Confusion matrices are plotted for each classifier to visualize the classification performance. In addition, the accuracy, precision, recall, and F1-scores are compared across all models using bar plots.

# 6. Results
### Accuracy Scores:
 *Logistic Regression:* 97%
 *Decision Tree:* 96.5%
 *Random Forest:* 95.5%
 *SVC:* 97%
 *KNN:* 96.5%
#### F1-Scores: Similar performance is observed across classifiers, with Logistic Regression and SVC slightly outperforming others.

## Requirements
Python 3+

### Required Libraries:
pandas

numpy

scikit-learn

seaborn

matplotlib

### Clone the repository:
git clone 
