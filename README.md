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

## Cluster Insights:
All customers are divided into two clusters, each representing distinct characteristics.
<p align="center">
  <img width="841" height="704" alt="Cluster Visualization using PCA" 
       src="https://github.com/user-attachments/assets/548b83cd-1679-442c-b5e0-ed2526018122" />
  <br>
  <em>Figure 1. Customer Segmentation Visualization using PCA</em>
</p>

1. **Cluster 0: Mature & Financially Stable Customers**

This cluster represents predominantly mature customers (average age ~45) with relatively stable and well-planned financial behavior.
They maintain moderate-to-high account balances (avg. ~$5,142) and show consistent transaction patterns, with transaction amounts averaging ~$255 and durations generally longer, indicating more cautious and deliberate financial decisions.

Although dominated by financially stable customers, this group still shows wide variability in balance, transaction size, and transaction duration, reflecting diverse financial capacities and transaction complexities.
The strong preference for Branch channel usage suggests a tendency toward personal interaction and trust-based banking services.

**Business Insight:**
This segment is ideal for long-term investment products, premium banking services, and loyalty programs.

2. **Cluster 1: Younger & Transaction-Active Customers**

This cluster is characterized by relatively younger customers (average age ~44), with many coming from a student background.
They demonstrate slightly higher transaction activity than Cluster 0, with an average transaction amount of ~$258 and generally shorter transaction durations, reflecting more dynamic financial behavior.

Account balances remain financially stable (avg. ~$5,059), though slightly lower than Cluster 0, with broad variability across customers.
Despite their younger profile, Branch channel remains the dominant interaction method, indicating that face-to-face service is still highly valued even among younger customers.

**Business Insight:**
This segment is suitable for entry-level investment products, savings programs, financial education services, and growth-oriented customer development strategies.

## Model Performance Evaluation
The performance of the Decision Tree and Random Forest models was evaluated using standard classification metrics, including accuracy, precision, recall, and F1-score, to assess their predictive reliability.

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

Both Decision Tree and Random Forest models achieved excellent performance across all evaluation metrics (accuracy, precision, recall, and F1-score), indicating strong predictive capability and consistent classification of customer segments based on the generated cluster labels.

Hyperparameter tuning applied to the Random Forest model did not significantly change the evaluation metrics, as the baseline performance was already optimal. However, the tuning process improved model stability and generalization by selecting more robust parameter configurations, making the tuned model more reliable for real-world deployment.
