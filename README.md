# Bank Fraud Transaction Detection

This project aims to detect fraudulent transactions within a dataset of 2500 records by leveraging a combination of machine learning and statistical techniques. The goal is to identify and classify fraudulent transactions effectively, enabling organizations to mitigate risks and ensure the security of financial systems.

---

## Overview

To detect fraudulent transactions, the project employs four methodologies:
1. **K-means Clustering**: Identifies anomalies based on distance from centroids in an unsupervised learning approach.
2. **Logistic Regression**: Classifies transactions as fraud or non-fraud using supervised learning.
3. **Isolation Forest**: Highlights anomalous transactions using tree-based partitioning.
4. **XGBoost Classifier (XGBClassifier)**: Provides gradient boosting-based supervised learning for classification tasks.

These methodologies are integrated into a comprehensive pipeline for detecting and analyzing fraud.

---

## Libraries and Tools Used

The project utilizes the following Python libraries:
- **Data Manipulation**:
  - `pandas`
  - `numpy`
- **Visualization**:
  - `matplotlib`
  - `seaborn`
  - `mpl_toolkits.mplot3d` (`Axes3D`)
- **Data Preprocessing**:
  - `StandardScaler`
  - `OneHotEncoder`
- **Machine Learning Models**:
  - `KMeans`
  - `IsolationForest`
  - `LogisticRegression`
  - `XGBClassifier`
  - `DBSCAN`
- **Evaluation Metrics**:
  - `classification_report`
  - `confusion_matrix`
  - `accuracy_score`
  - `roc_curve`
  - `roc_auc_score`
- **Other Tools**:
  - `train_test_split`
  - `datetime`
  - `warnings`

---

## Features

- **K-means Clustering**: Identifies potential fraudulent transactions through unsupervised anomaly detection.
- **Logistic Regression**: Provides a supervised learning approach for classification.
- **Isolation Forest**: Detects anomalies based on tree-based partitioning.
- **XGBoost Classifier**: Leverages gradient boosting to provide accurate classification of fraudulent transactions.
- **Visualization**: Generates insightful plots for data exploration and results interpretation.

---

## Installation

### Prerequisites

Ensure you have Python installed along with the required libraries. Install the dependencies using the following command:

```bash
pip install -U scikit-learn pandas numpy matplotlib seaborn xgboost
```

---

## Usage

1. Clone the repository to your local system:
   ```bash
   git clone https://github.com/databytobi/bank_fraud_transaction_detection.git
   ```
2. Run the main script to preprocess the data, train models, and evaluate performance:
   ```bash
   python main.py
   ```

---

## Project Structure

```
bank_fraud_transaction_detection/
│
├── data/                  # Dataset files
├── notebooks/             # Jupyter notebooks for exploration and visualization
├── src/                   # Source code
│   ├── data_processing.py # Data preprocessing scripts
│   ├── anomaly_detection.py # Scripts for K-means and Isolation Forest
│   ├── classification.py  # Logistic Regression and supervised learning
│   ├── evaluation.py      # Evaluation scripts
│   └── visualization.py   # Plotting and results visualization
├── tests/                 # Unit tests
├── main.py                # Main script to run the project
├── README.md              # Project documentation
└── requirements.txt       # Python dependencies
```

---

## Evaluation Metrics

The following metrics are used to evaluate the models:
- **Accuracy Score**: Measures the overall accuracy of the model.
- **Classification Report**: Provides precision, recall, and F1-score.
- **Confusion Matrix**: Displays the performance of the classification model.
- **ROC Curve**: Visualizes the trade-off between sensitivity and specificity.
- **AUC-ROC Score**: Quantifies the ability of the model to distinguish between classes.

---

## Contributing

Contributions are welcome! If you have ideas for improvements or additional features, feel free to submit a pull request or open an issue.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgements

- Scikit-learn and XGBoost for providing tools for anomaly detection and classification.
- Pandas and NumPy for data manipulation.
- Matplotlib and Seaborn for visualization.
