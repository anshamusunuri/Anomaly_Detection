# Anomaly_Detection

This project focuses on detecting anomalies in time series data through advanced machine learning techniques. The goal is to accurately identify unusual patterns that may signal potential issues, making the model applicable to fields such as fraud detection, equipment failure prediction, and network security.

Project Highlights:
Data Preprocessing and Normalization: The raw time series data was cleaned, and missing values were addressed. Data was normalized, and trend/seasonality components were removed, ensuring the model could effectively capture deviations from normal patterns.

Exploratory Data Analysis (EDA): Extensive EDA was conducted to uncover normal behaviors and identify potential anomalies in the dataset. Time-based trends and sudden deviations were visualized, providing insights into the structure of the data.

Unsupervised Learning Algorithms: Three key algorithms were applied for anomaly detection:

KMeans Clustering: Used to group data into clusters and identify anomalies based on their distance from the cluster centroids. This technique helped detect points that deviated significantly from typical behavior.

Isolation Forest: Leveraged to isolate anomalies by randomly partitioning the data. Points that were separated early in the partitioning process were considered anomalies, making this method efficient and highly effective for detecting outliers.

Local Outlier Factor (LOF): Implemented to measure the local deviation of a data point with respect to its neighbors. LOF helped detect both global and local anomalies, improving the model's sensitivity to unusual patterns.

Feature Engineering: Created rolling statistics, moving averages, and lag features to capture underlying temporal trends. These enhanced features improved the model's ability to detect both abrupt changes and gradual anomalies in the time series.

Model Evaluation and Optimization: Performance was evaluated using precision, recall, and F1-score to ensure the model balanced accuracy in detecting true anomalies while minimizing false alarms. Fine-tuning of hyperparameters via grid search ensured optimal performance across all algorithms.

Anomaly Visualization: The detected anomalies were plotted against the original time series data, providing clear, actionable insights on when and where these unusual events occurred.

This project demonstrates how clustering techniques like KMeans, along with robust methods like Isolation Forest and LOF, can be effectively employed for anomaly detection
