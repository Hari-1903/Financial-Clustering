# Financial Clustering: Predicting Profitability
Understanding the financial health of companies is crucial for investors, analysts, and stakeholders alike. One key metric in assessing a company's performance is its net income, which reflects the profitability of its operations after accounting for all expenses.

The primary focus of this project lies in utilizing unsupervised learning techniques, specifically clustering, to discern patterns within the dataset and identify the most suitable algorithm for predicting whether a company has recorded a net profit or net loss. To facilitate this analysis, we will transform the Net Income column into a binary representation, where a value of 1 signifies profit and 0 denotes loss. By undertaking this transformation, we aim to build a model capable of accurately categorizing companies based on their financial performance.

The dataset for this project is taken from [Kaggle](https://www.kaggle.com/datasets/dgawlik/nyse)

## Aproach
- **Data Collection**: Obtain dataset from Kaggle, comprising financial metrics of NYSE-listed companies from 2012 to 2016.
- **Preprocessing**: Clean data, handle missing values, and ensure consistency in features such as revenue, expenses, assets, liabilities, cash flow, earnings per share (EPS), and various financial ratios.
- **Feature Engineering**: Select pertinent features that could impact profitability, normalize or scale them as needed for uniform representation.
- **Clustering Techniques**: Employ unsupervised learning algorithms like k-means and hierarchical clustering models to uncover inherent patterns within the dataset.
- **Model Evaluation**: Assess algorithmic performance by comparing the clustering results in segregating data points to determine the most effective method for categorizing companies based on their financial performance.
- **Interpretation**: Analyze clustering results to gain insights into the financial characteristics distinguishing profitable companies from those operating at a loss. Examine cluster centroids or medoids to identify key features contributing to profitability.

## Results
In conclusion, the analysis highlights a notable discrepancy in the accuracy of predicting profit compared to predicting loss, attributed to the substantial disparity in data distribution between profitable and non-profitable companies (1: 1679 vs 0: 102). The **Complete-link Agglomerative Clustering model demonstrates superior performance in predicting loss**, while **KMeans Clustering emerges as the optimal choice for predicting profit**, although Ward-link Agglomerative Clustering also yields commendable results.

## Future Developments

To potentially improve results, exploring additional techniques like Principal Component Analysis (PCA) or hyperparameter tuning could be beneficial. PCA and hyperparameter tuning can enhance clustering by reducing dimensionality, mitigating noise, and optimizing algorithm parameters, leading to more accurate and reliable results.
