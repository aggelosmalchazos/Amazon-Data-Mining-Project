# Amazon-Data-Mining-Project

Contributors:
Pavlos Karagiorgos
Aggelos Malchazos
Semeli Mouti

This project involves a comprehensive e-commerce analysis using the **Amazon Product Dataset**. The objective is to perform data exploration, feature engineering, and apply various machine learning tasks including clustering, recommendation systems, and sentiment analysis.

---
This is a project built using Python and JupyterNotebook. 

---

## Part 1: Pre-processing & Feature Engineering

### 1. Data Preparation

The dataset is sourced from **Hugging Face** in JSON format.


**Extraction:** Convert JSON files into 5 separate CSV files (one per category).



**Streaming:** Use the `datasets` library with `streaming=True` to handle the large dataset size.



**Cleaning:** Handle missing values, normalize prices, and perform initial text preprocessing.



### 2. Data Exploration (EDA)

Visualize the following using Matplotlib, Seaborn, or Plotly:


**Rating Distribution:** Distribution of product ratings within each category.


**Top Products:** Identify the top 5 best-selling products per category based on review count.



**Trends:** Line plots showing the evolution of average ratings over months or years.



### 3. Advanced Feature Engineering

Develop a **Final Sentiment Score** using one of the following methods:


**Weighted Combination:** Blending VADER/Hugging Face sentiment scores with normalized 1-5 star ratings.








**Rating-Adjusted Sentiment:** Amplifying or decreasing sentiment scores based on star ratings (e.g., ±0.2 factor).



**Optional Metrics:** Price-per-feature normalization and weighted ratings adjusted by review volume.








---

##  Part 2: Machine Learning Tasks

### Task 1: Clustering for Product Grouping

Group similar products based on price, description, and ratings.


**Vectorization:** TF-IDF for product descriptions.



**Algorithm:** K-Means (with Elbow Method) or DBSCAN.



**Evaluation:** Silhouette Score and visualization using PCA or t-SNE.



### Task 2: Recommendation System

Implement a system to suggest products based on past behavior.


**Collaborative Filtering (CF):** User-based and Item-based filtering using Cosine Similarity.


**Content-Based Filtering (CBF):** Using **Word2Vec** embeddings for product descriptions.



**Hybrid Approach:** A weighted average of CF and CBF scores.








### Task 3: Sentiment Classification

Classify reviews as Positive, Negative, or Neutral.


**Features:** TF-IDF, Word2Vec, or FastText embeddings.



**Models:** Naive Bayes, KNN, Random Forest, and optional Deep Learning (LSTM/BERT).



**Evaluation:** 10-fold Cross-Validation with metrics including F1-Score, Precision, Recall, and Accuracy.



### Task 4: Bonus - Frequent Pattern Mining

Discover products frequently bought together.


**Algorithm:** **Apriori** to identify frequent itemsets and association rules.



**Metric:** **Lift** to measure the strength of association.



---
