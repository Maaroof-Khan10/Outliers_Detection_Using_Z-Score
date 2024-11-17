# Outlier Detection Using Z-Scores and KMeans Clustering

This project demonstrates how to detect outliers in a dataset using Z-scores, with the help of KMeans clustering. It generates synthetic data, applies KMeans clustering to segment the data into two groups, and then uses the Z-score method to identify outliers within each cluster.

The Z-score is used to measure how many standard deviations a data point is from the mean. Points with a Z-score greater than 3 are typically considered outliers. In this notebook, I apply this technique on a synthetic dataset, visualize the clustering results, and identify the outliers.

## Project Structure

- `Outlier Detection.ipynb`: The main Jupyter notebook where we perform data generation, clustering, and outlier detection using Z-scores.
- `README.md`: This file.

## Requirements

Before running this project, make sure you have the following Python libraries installed:

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

You can install them using `pip`:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

## Running the Notebook

To run the Jupyter notebook, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/Maaroof-Khan10/Outliers_Detection_Using_Z-Score.git
   ```

2. Navigate to the project directory:

   ```bash
   cd Outliers_Detection_Using_Z-Score
   ```

3. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

4. Open the `Outlier Detection.ipynb` file and run the cells.

## Overview of the Notebook

### 1. **Introduction**
   In this section, we start with the concept of outlier detection using Z-scores and KMeans clustering.

### 2. **Importing Libraries**
   We import the necessary libraries for data manipulation, visualization, and clustering.

### 3. **Generating Synthetic Data**
   Now we generate a synthetic dataset using the `make_blobs` function, add some outliers, and organize the data into a DataFrame for easy manipulation.

### 4. **Visualizing the Data**
   A scatter plot is used to visualize the synthetic data before clustering. The outliers are not yet identified at this stage.

### 5. **Clustering the Data with KMeans**
   KMeans clustering is applied to segment the data into two clusters. The results are stored in the `Y` column, indicating which cluster each data point belongs to.

### 6. **Outlier Detection Using Z-Scores**
   For each cluster, we calculate the Z-scores for both features (X1 and X2). Points with a Z-score greater than 3 are considered outliers. I output the detected outliers for each cluster.

### 7. **Visualizing the Outliers**
   A final visualization shows the clusters with the outliers marked in red and green. The means of each cluster are also indicated to provide context.
   
   ![D2](https://github.com/user-attachments/assets/a7e7e5dd-115a-45af-bb15-cadd1fd95fcc)

### 8. **Conclusion**
   A brief summary of the method and how it can be applied to detect outliers in clustered data.

## Purpose and Use Cases

This technique can be applied to various domains, such as:

- **Anomaly detection** in financial transactions, fraud detection, or sensor data.
- **Quality control** in manufacturing, where outlier products might indicate defects.
- **Data preprocessing** for machine learning, where removing outliers can improve model performance.

---

### Additional Notes:

- Feel free to modify the notebook for your own datasets and experiment with different clustering algorithms or outlier detection methods.

---
