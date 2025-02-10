# Income-Age Clustering Analysis

## Overview

This project demonstrates the application of K-Means clustering to analyze and segment individuals based on their age and income data. The analysis helps identify natural groupings in the data that could be valuable for marketing strategies, customer segmentation, or demographic studies.

## Features

- Data preprocessing and visualization
- Implementation of K-Means clustering
- Feature scaling using MinMaxScaler
- Cluster visualization with centroids
- Elbow method implementation for optimal cluster selection

## Dependencies

The project requires the following Python libraries:

- scikit-learn
- numpy
- pandas
- matplotlib
- MinMaxScaler from sklearn.preprocessing

## Dataset

The project uses a dataset (`income.csv`) containing the following columns:

- Name: Individual's name
- Age: Person's age
- Income($): Annual income in dollars

## Code Structure

The notebook contains several key sections:

1. **Data Loading and Initial Visualization**

   - Loading the dataset
   - Initial scatter plot of age vs income

2. **K-Means Implementation**

   - Creating KMeans instance
   - Fitting and predicting clusters
   - Adding cluster labels to the dataset

3. **Data Scaling and Visualization**

   - Normalizing age and income data
   - Visualizing clusters with different colors
   - Plotting centroids

4. **Elbow Method**
   - Implementation of elbow method
   - Plotting SSE vs number of clusters
   - Determining optimal number of clusters

## Results

The analysis reveals three distinct clusters in the data:

- Cluster 0: Young individuals with moderate income
- Cluster 1: Middle-aged individuals with high income
- Cluster 2: Older individuals with varying income levels

## Usage

1. Ensure all required libraries are installed
2. Load the notebook in Jupyter
3. Run all cells sequentially
4. Modify parameters as needed for your analysis

## Visualization

The notebook includes several visualizations:

- Initial scatter plot of age vs income
- Clustered data with color-coded groups
- Centroids marked on the plot
- Elbow curve for optimal cluster selection

## Future Improvements

- Add more features for clustering
- Implement other clustering algorithms for comparison
- Add statistical analysis of clusters
- Include more validation metrics

## Contributing

Feel free to fork this project and submit pull requests with improvements.

## License

This project is open-source and available under the MIT License.
