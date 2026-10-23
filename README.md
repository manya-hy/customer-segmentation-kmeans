# Customer Segmentation Using K-Means Clustering

## 1. Project Overview

This project applies unsupervised machine learning to group mall customers according to their age, annual income, and spending score.

The objective is to identify customer segments with similar characteristics and demonstrate how clustering can support customer behavior analysis and marketing decisions.

## 2. Problem Statement

Understanding customer behavior helps businesses develop more effective marketing strategies. This project uses the K-Means clustering algorithm to group customers based on selected numerical features and analyze the characteristics of each segment.

## 3. Objectives

* Load and explore customer data.
* Perform data cleaning and exploratory data analysis.
* Standardize numerical features using StandardScaler.
* Determine a suitable number of clusters using the Elbow Method.
* Evaluate clustering using the Silhouette Score.
* Train a K-Means clustering model.
* Visualize customer segments.
* Analyze cluster characteristics.
* Export customer assignments and analytical results.

## 4. Dataset

**Dataset:** Mall Customer Segmentation Data

**Source:** [Kaggle — Customer Segmentation Tutorial in Python](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)

The commonly used dataset contains 200 customer records and five columns.

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| CustomerID             | Unique customer identifier            |
| Gender                 | Recorded customer gender              |
| Age                    | Customer age                          |
| Annual Income (k$)     | Annual income in thousands of dollars |
| Spending Score (1-100) | Customer spending score               |

The model uses Age, Annual Income, and Spending Score as input features.

## 5. Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

## 6. Methodology

1. Load and inspect the dataset.
2. Check for missing values and duplicate records.
3. Perform exploratory data analysis.
4. Select relevant numerical features.
5. Scale the features using StandardScaler.
6. Apply the Elbow Method to study inertia for different cluster counts.
7. Compare Silhouette Scores.
8. Train the K-Means model.
9. Visualize the resulting clusters.
10. Analyze cluster profiles.
11. Export results and visualizations.

## 7. Evaluation Metrics

### Inertia

Measures the sum of squared distances between customers and their assigned cluster centers. Lower inertia indicates more compact clusters, but it generally decreases as the number of clusters increases.

### Elbow Method

Helps identify a reasonable cluster count by examining where additional clusters provide diminishing reductions in inertia.

### Silhouette Score

Measures how well-separated the clusters are. A higher score generally indicates better-defined clusters, although the result must be interpreted alongside the dataset and project objective.

## 8. Results

The final model uses the selected number of clusters and groups customers according to the three numerical features.

The notebook generates:

* An Elbow Method graph.
* A Silhouette Score comparison.
* A customer cluster scatter plot.
* Cluster profile visualizations.
* Customer assignments and cluster summaries.

The exact Silhouette Score, customer counts, and segment characteristics should be taken from the executed notebook outputs.

## 9. Applications

Customer segmentation can help businesses:

* Understand differences in customer spending behavior.
* Identify groups for targeted marketing campaigns.
* Compare customer groups by income and age.
* Explore opportunities to improve customer engagement.

These are potential applications rather than guaranteed business outcomes.

## 10. Project Structure

```text
Week4_ML_Customer_Segmentation/
├── data/
│   └── Mall_Customers.csv
├── outputs/
│   ├── customer_segments.csv
│   ├── cluster_profiles.csv
│   ├── cluster_centers.csv
│   ├── silhouette_results.csv
│   └── generated_visualizations.png
├── customer_segmentation.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

The actual outputs folder may contain several separate visualization files.

## 11. Installation and Execution

1. Download or clone the project repository.
2. Download the dataset from Kaggle.
3. Place `Mall_Customers.csv` inside the `data` folder.
4. Install the dependencies:

```bash
pip install -r requirements.txt
```

5. Open the project folder in JupyterLab.
6. Open `customer_segmentation.ipynb`.
7. Run the notebook cells in order.

## 12. Limitations

* The dataset is small and may not represent all mall customers.
* Results depend on feature selection, scaling, and the chosen number of clusters.
* Spending-group labels use illustrative thresholds.
* Customer segments describe patterns in the available data and do not establish causal relationships.
* Real business decisions require validation against relevant business data.

## 13. Conclusion

This project demonstrates an end-to-end unsupervised machine learning workflow using K-Means clustering. It combines data preprocessing, exploratory analysis, cluster selection, evaluation, visualization, and customer profiling to explore customer behavior.

## Disclaimer

This project is developed for educational purposes. Its findings are illustrative and should be validated before being used for actual business decisions.
