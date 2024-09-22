# Bank Marketing Insights Analysis

## Project Overview
This project provides insights into the effectiveness of marketing campaigns for a Portuguese bank. The analysis revolves around a dataset that contains details of campaigns conducted via phone calls, with the goal of determining whether a client agreed to subscribe to a term deposit. The target variable is binary, indicating "yes" or "no" based on the client's response.

### Dataset Description:
The dataset contains the following key information:
- **Client Demographics:** Age, job type, marital status, and education level.
- **Financial Information:** Whether the client has housing or personal loans, and whether they have defaulted on credit.
- **Campaign Details:** Number and outcome of previous campaigns, type of contact, and timing of the last contact.
- **Economic Indicators:** Employment variation rate, consumer price index, Euribor 3-month rate, and more.

## Steps in the Analysis:

### 1. Data Preprocessing:
- **Feature Encoding:** Categorical variables like job, marital status, and education are label-encoded for machine learning compatibility.
- **Scaling:** Numeric features are standardized to ensure uniformity in the dataset, using the `StandardScaler`.
- **Dimensionality Reduction:** Principal Component Analysis (PCA) is employed to reduce the dimensionality of the data for easier visualization and clustering.

### 2. Clustering Techniques:
- **KMeans Clustering:** A segmentation technique used to divide clients into groups based on similar characteristics. The optimal number of clusters is determined using the silhouette score.
- **Agglomerative Clustering:** Another clustering technique is applied to see hierarchical relationships among clients.

### 3. Visualizations:
- **Correlation Heatmaps:** Visual representations of correlations between features, such as age, job, and the likelihood of subscribing to a term deposit.
- **PCA Plots:** Dimensionality reduction to visualize high-dimensional data.
- **Histograms and Bar Plots:** To explore the distribution of individual features.

## Key Insights:
- Clients' age, job type, and education level significantly influence their likelihood of subscribing to a term deposit.
- Previous campaign outcomes (success or failure) are strongly correlated with future success in campaigns.
- Economic conditions, as reflected by variables like the Euribor 3-month rate, also affect clients' decisions.

## Conclusion:
The analysis provides a detailed understanding of factors affecting clients' responses to marketing campaigns. By segmenting customers using clustering algorithms, we can target specific groups more effectively in future campaigns, optimizing the marketing strategy.

## How to Run the Code:
1. Clone the repository.
   ```bash
   git clone <github.com/navin1111/Bank-Market-Analysis>
2. Install the required packages from requirements.txt
   ```bash
   pip install -r requirements.txt
3. Run the Jupyter Notebook to explore the analysis.
   
