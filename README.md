# Predict Customer Personality to Boost Marketing Campaign
<br>

- **Tools** : Google Colabs<br>
- **Programming Language** : Python <br>
- **Dataset** : Rakamin Academy <br>
- **Libraries** : Pandas, NumPy, Sklearn <br>
- **Visualization** : Matplotlib, Seaborn, yellow-brick <br>
- **Dataset** : Disediakan oleh Rakamin Academy <br>
- **Skillset** :  Analytical Thinking, Business understanding, Python Data Preprocessing, Machine Learning, Clustering<br>
- **Notebook** : <br>

<br>
<br>

----

## 📂 **Problem Statement**

### Introduction
Understanding customer behavior is crucial to adjust the company's marketing strategy. By understanding customer preferences, needs, and purchasing patterns, the company can provide a better experience, increase satisfaction, and overall sales performance. Clustering approach helps in grouping customers and provides valuable insights for more effective marketing strategies.

### Goals
The goal of analyzing customer profiles and behaviors using clustering approach is to understand customers better, provide more personalized services, improve sales performance, and build strong relationships with customers.

### Objective
- Creating a machine learning model that can categorize customers into different segments based on their characteristics or behaviors.
- Extracting deeper insights into customer profiles and behaviors.
- Determining effective business strategies from clustering results.
<br>
<br>

---

## 📂 **Data Modeling with K-Means Clustering**
### Pre-processing
Before performing data modeling, there are several stages of data pre-processing that need to be done:
- **Unnecessary features** for the model will be **removed** to focus the data more.
- Categorical features will be **encoded** to be processed by machine learning algorithms.
- Feature **standardization** will be conducted to ensure uniform data scale and avoid bias in the model.
<br>

### Modelling
After completing data pre-processing, the next step is to use the **Principal Component Analysis (PCA)** method. PCA is used to reduce the dimensionality of data while retaining significant information. By reducing the data dimensions, it can optimize model performance and address multicollinearity issues among features. Furthermore, an important step in this process is determining the best number of clusters. In this analysis, **Distortion Score and Elbow Method** are used to select the optimal number of clusters. Based on the analysis results, **the optimal number of clusters found is 4**.
<br>
<br>
After determining the optimal number of clusters, **clustering is performed using the K-means algorithm**. This algorithm will group data into clusters based on feature similarity. By performing clustering, it can identify patterns or groups within the data and understand the characteristics of each cluster.
<br>
<br>
From the plot of the modeling results and data grouping using clustering methods, it is observed that **the formed clusters are well separated** and classify data into different groups. This indicates that the clustering algorithm used successfully distinguishes and categorizes data based on their characteristics.
<br>

### Evaluation
Evaluation of the model results using **Silhouette Score** recommends that the optimal number of clusters is 4. This recommendation is based on the fact that the Silhouette Score value for this number of clusters is the highest, which is 0.540. Silhouette Score is an evaluation metric that depicts how well objects within a cluster are grouped within their own dataset compared to other clusters. The higher the Silhouette Score value, the better the separation of these clusters.
<br>
<br>

---

## 📂 **STAGE 4: Customer Personality Analysis**
Customer Personality Analysis aims to **understand the differences and similarities between these clusters, as well as identify unique characteristics that each group may possess**. With a deeper understanding of the characteristics among clusters, companies can take more appropriate actions and direct more specific business strategies for each customer group.
<br>
<br>
Based on deeper analysis results, the average/majority characteristics of each cluster can be identified based on customer transaction patterns and can be grouped into several categories.
<br>
- **Cluster 0**
    - The highest transaction and spending figures are mostly 25 transactions of around Rp900,000 per month.
    - The income is quite high, mostly Rp65,215,000 per year.
    - The conversion rate is moderate, at 4.5%.
    - The majority age is 50 years old. 
    - Kategori : **"*High-Transaction Moderate-Spending Group*" - High Customer B** <br>
<br>

- **Cluster 1**
    - The lowest transaction and spending figures are mostly only 7 transactions and Rp.150,000 per month.
    - The lowest income, mostly Rp.33,297,500 per year.
    - The lowest conversion, which is 1%.
    - The majority age is 35 years old.
    - Kategori : **"*Low-Transaction Low-Spending Group*" - Low Customer** <br>
<br>
    
- **Cluster 2**
    - Transaction numbers and spending are quite high, with the majority being 20 transactions and Rp.1,400,000 per month.
    - The highest income, mostly Rp.80,000,000 per year.
    - The highest conversion rate, which is 9%.
    - The majority are 40 years old.
    - Kategori : **"*High-Income High-Conversion Group*" - High Customer A** <br>
<br>

- **Cluster 3**
    - Transaction and spending figures are moderate, with the majority being 10 transactions and Rp.180,000 per month.
    - Income is moderately sufficient, with the majority being Rp.40,000,000 per year.
    - Conversion rate is moderately sufficient, at 1.8%.
    - The majority are 48 years old.
    - Kategori : **"*Moderate-Transaction Low-Spending Group*" - Moderate Customer**<br>
<br>
