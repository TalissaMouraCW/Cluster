# Customer Base Segmentation with K-Means Clustering

This project demonstrates customer segmentation using **unsupervised machine learning** techniques, specifically the **K-Means algorithm**. The goal is to group customers with similar characteristics to better understand their behavior and preferences, allowing for more personalized marketing strategies.

## Table of Contents
- [Project Overview](#project-overview)
- [Getting Started](#getting-started)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Data Exploration](#data-exploration)
- [Clustering Analysis](#clustering-analysis)
- [Visualization](#visualization)
- [Conclusion](#conclusion)

## Project Overview
This project is geared towards understanding customer differences by segmenting a customer base using **K-Means clustering**. The dataset used contains fictitious data that represents typical customer features, such as age, monthly spending, subscription duration, and more. The segmentation helps identify different customer groups with similar characteristics, offering insights that can be used by marketing teams to design targeted campaigns.

## Getting Started
To get started with this project, clone the repository and follow the installation steps below.

## Prerequisites
Before running the project, ensure you have the following Python packages installed:
- `threadpoolctl==3.1.0`
- `numpy`
- `pandas`
- `seaborn`
- `matplotlib`
- `scikit-learn`
- `scipy`

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/your-repository-name.git
   ```
2. Navigate to the project directory:
   ```bash
   cd your-repository-name
   ```
3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Data Exploration
The dataset contains various features such as:
- **Age**: Customer age
- **Monthly Spending**: Average monthly expenditure
- **Subscription Duration**: Number of years subscribed to the service
- **Usage Rate**: How frequently the customer uses the product/service
- **Support Tickets**: Number of support tickets opened
- **Cancelled**: Indicates whether the customer canceled their subscription

### Key Steps:
1. **Checking for Null Values**: Ensures there are no missing data points.
2. **Identifying Outliers**: Uses boxplots to detect outliers, which can impact clustering results.
3. **Correlation Analysis**: Analyzes the relationships between variables to identify multicollinearity.

## Clustering Analysis
The clustering process involves:
- **Standardization**: Scaling data for better clustering performance.
- **Determining Optimal K**: Using the **Elbow Method** and **Silhouette Analysis** to identify the ideal number of clusters.
- **Clustering with K-Means**: Testing various values of K (number of clusters) and analyzing the results.

### Key Observations:
- **Cluster 0**: Customers who did not cancel their subscription, typically younger with lower spending.
- **Cluster 1**: Customers who canceled their subscription, generally older with higher spending.
- **Cluster 2**: A mixed group with characteristics close to the dataset's average.

## Visualization
Various plots are generated to visualize the clustering results:
1. **2D Scatter Plot**: Visualizes customer age versus monthly spending across clusters.
2. **3D Scatter Plot**: Adds subscription duration for deeper analysis.
3. **PCA Visualization**: Reduces dimensionality to show clusters in 2D using Principal Component Analysis.
4. **t-SNE Visualization**: Another dimensionality reduction technique for visualizing high-dimensional data in 2D.

## Conclusion
This project provides valuable insights into customer segmentation using open-source tools like Python and scikit-learn. By grouping customers based on their behavior, marketing teams can tailor campaigns, products, and services to better meet the needs of different customer segments.

Feel free to explore the code, experiment with different K values, and adapt the approach to your specific dataset and business needs.

---

You can adjust the project description, repository URL, and other specific details as needed.
