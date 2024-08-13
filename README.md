# heart-disease-clustering

## Project Overview
This project analyzes the Heart Disease dataset from the UCI Machine Learning Repository using unsupervised learning techniques. The goal is to identify patients with high risk of developing heart disease and uncover risk factors associated with heart disease.

## Dataset
The dataset contains 303 instances with 14 attributes including:
- Age
- Sex
- Chest pain type
- Blood pressure
- Serum cholesterol
- And other medical indicators

The target variable indicates the presence or absence of heart disease.

## Methodology
The analysis follows these main steps:
1. Exploratory Data Analysis (EDA)
2. Data Preprocessing
3. Clustering Analysis (K-means, Hierarchical, DBSCAN)
4. Dimensionality Reduction and Visualization (PCA, t-SNE)
5. Gaussian Mixture Models
6. Clustering Evaluation
7. Comparison of Different Techniques

## Key Findings
K-means Performance:

The Silhouette Score is positive but relatively low (0.127). A score closer to 1 indicates better-defined clusters.
The Davies-Bouldin Index is 2.289. Lower values indicate better clustering.

DBSCAN Performance:

DBSCAN failed to find any meaningful clusters in the dataset.
This suggests that the data doesn't have clear density-based clusters, or the chosen parameters (eps and min_samples) were not suitable for this dataset.

GMM Performance:

The Silhouette Score is very low (0.029), indicating poorly defined or overlapping clusters.
The Davies-Bouldin Index is higher than K-means, suggesting worse cluster separation.

Conclusion:
- K-means clustering performed best among the tested algorithms, although its performance suggests that clear, well-defined clusters are not present in the data.
- DBSCAN was unable to find meaningful clusters, indicating a lack of clear density-based structures in the dataset.
- Gaussian Mixture Models provided insights into potential risk factors but showed significant overlap between components.
- The difficulty in finding clear clusters suggests that heart disease risk factors interact in complex ways that don't naturally fall into distinct groups.

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

## Repository Structure
- `heart_disease_clustering.ipynb`: Jupyter notebook containing the full analysis
- `README.md`: This file, providing an overview of the project


## How to Run
1. Clone this repository
2. Install the required packages: `pip install -r requirements.txt`
3. Open and run the Jupyter notebook `heart_disease_analysis.ipynb`

