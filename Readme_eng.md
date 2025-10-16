# **Customer Clustering**

## **1\. Introduction**

This project aims to apply unsupervised machine learning techniques to perform customer segmentation. The analysis seeks to identify behavioral patterns in consumer data and support more effective marketing strategies.

## **2\. Problem Solved**

Companies often lack clarity about who their best customers are, which ones show high engagement, and which have low purchasing potential. This makes it difficult to design targeted marketing campaigns and increases customer acquisition costs.

The problem addressed in this project is the identification of different customer profiles based on demographic and consumption behavior data.

## **3\. Problem-Solving Approach**

An exploratory data analysis (EDA) was first performed to understand variable distributions and detect potential patterns. Then, the K-Means algorithm — a widely used statistical model in customer segmentation — was applied.

The problem falls under the unsupervised learning category, where the model automatically identifies similarities between customers and groups them into clusters.

Clustering aims to group individuals so that those in the same cluster are more similar to each other than to those in other clusters.  In this project, the goal of applying K-Means was to determine which segment each customer belongs to, enabling the characterization of distinct behavioral profiles.

Additionally, it was necessary to define the optimal number of clusters to represent the data in a way that is meaningful for business insights.  To achieve this, validation metrics and techniques were used — mainly the Elbow Method and Silhouette Analysis, which helped determine the most appropriate segmentation.

## **4\. Project Structure**

├── Dados/                               \# Folder containing datasets    
├── Clusterização\_de\_Clientes.ipynb      \# Modeling and evaluation of machine learning models    
├── Readme/                              \# Project explanation  

## **5\. Technologies Used**

The main technologies and libraries used were:

* Pandas → data manipulation, cleaning, and transformation into DataFrames.

* NumPy → efficient numerical computations, including vector and matrix operations.

* Matplotlib / Pyplot → creation of basic and customizable plots for data analysis.

* Seaborn → advanced and intuitive statistical visualizations for easier interpretation.

* SciPy → applied to statistical operations, advanced mathematical functions, and preprocessing.

* Scikit-learn (Sklearn) → main machine learning library, used for clustering algorithms (K-Means, hierarchical clustering) and evaluation metrics.

* Yellowbrick → used to generate specific graphical visualizations for model evaluation, such as the Elbow Method and Silhouette Analysis.

## **6\. Results**

Based on Elbow Graph and Silhouette Analysis, the optimal number of clusters was determined to be five customer segments.

The analysis revealed distinct characteristics among these segments, summarized as follows:

* Cluster 0 (40.5%): Predominantly female, average age 42, average income 55k, score around 49\. Represents the regular group, i.e., the majority of the customer base.

* Cluster 1 (19.5%): Mostly female, average age 32, high average income (86k), and high score (82). Considered a strategic segment with high purchasing power and strong engagement.

* Cluster 2 (11.0%): Mostly young women (25 years old), low income (26k), but high score (79). Represents potential customers, as they show high purchasing intent despite current low income.

* Cluster 3 (17.5%): Predominantly male, average age 41, high income (88k), but very low score (17). Despite their purchasing power, low engagement makes this group a low strategic priority.

* Cluster 4 (11.5%): Mainly older women (45 years old), low income (28k), and low score (20). This segment is less attractive for marketing strategies due to low engagement and limited consumption capacity.

