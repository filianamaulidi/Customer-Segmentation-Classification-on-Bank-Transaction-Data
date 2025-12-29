# Customer Segmentation Classification on Bank Transaction Data
An end-to-end machine learning pipeline for discovering customer segments and predicting customer groups from bank transaction data.

This project demonstrates an end-to-end machine learning pipeline that transforms raw, unlabeled bank transaction data into actionable customer segments and a predictive classification model.

By combining unsupervised and supervised learning, the system is able to automatically discover customer groups and then predict the segment of new customers in real-world scenarios.

## What I Did?
+ Performed extensive data cleaning, feature engineering, and preprocessing.
+ Applied K-Means clustering to discover natural customer segments from unlabeled data.
+ Interpreted each cluster to build meaningful customer personas.
+ Used the clustering result as ground truth labels.
+ Built supervised classification models to predict customer segments using Decision Tree and Random Forest Algorithm.
+ Tuned the best model using hyperparameter optimization.
+ Exported trained models and datasets for deployment-ready usage.

## Key Contributions
- Solves the real-world problem of missing customer labels.
- Combines unsupervised and supervised learning into a single pipeline.
- Produces both business insights and predictive models.
- Models achieve excellent performance across multiple evaluation metrics.
- Ready for real-world usage: models and processed datasets are exported.

## Business Impact
This pipeline enables financial institutions to:
- Understand customer behavior patterns.
- Automatically assign new customers into meaningful segments.
- Support personalized marketing, product recommendation, and risk profiling.

## Tech Stack 🖥️:
Python, Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib, Yellowbrick

## Documentation:
<p align="center">
  <img width="841" height="704" alt="Cluster Visualization using PCA" 
       src="https://github.com/user-attachments/assets/548b83cd-1679-442c-b5e0-ed2526018122" />
  <br>
  <em>Figure 1. Customer Segmentation Visualization using PCA</em>
</p>

**Decision Tree Performance:**
| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 1.00      | 1.00   | 1.00     | 196     |
| 1     | 1.00      | 1.00   | 1.00     | 193     |
| **Accuracy** |   |   | **1.00** | **389** |
| **Macro Avg** | **1.00** | **1.00** | **1.00** | **389** |
| **Weighted Avg** | **1.00** | **1.00** | **1.00** | **389** |


**Random Forest Performance:**
| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 1.00      | 1.00   | 1.00     | 196     |
| 1     | 1.00      | 1.00   | 1.00     | 193     |
| **Accuracy** |   |   | **1.00** | **389** |
| **Macro Avg** | **1.00** | **1.00** | **1.00** | **389** |
| **Weighted Avg** | **1.00** | **1.00** | **1.00** | **389** |

**Random Forest Performance (Tuned):**
| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 1.00      | 1.00   | 1.00     | 196     |
| 1     | 1.00      | 1.00   | 1.00     | 193     |
| **Accuracy** |   |   | **1.00** | **389** |
| **Macro Avg** | **1.00** | **1.00** | **1.00** | **389** |
| **Weighted Avg** | **1.00** | **1.00** | **1.00** | **389** |
