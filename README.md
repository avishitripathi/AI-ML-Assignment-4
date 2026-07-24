# Breast Cancer Classification using K-Nearest Neighbors (KNN)

## Objective

The objective of this project is to develop a K-Nearest Neighbors (KNN) classification model to predict whether a breast tumor is Malignant or Benign based on diagnostic measurements.

## Dataset

The Breast Cancer Wisconsin Diagnostic Dataset was obtained from Kaggle.

Dataset Link: https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data

The dataset has not been uploaded to this repository.

## Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Methodology

1. Loaded the Breast Cancer Wisconsin Diagnostic Dataset using Pandas.
2. Displayed the first five records.
3. Identified the numerical features and the target variable.
4. Displayed dataset information and summary statistics.
5. Checked for missing values.
6. Removed unnecessary columns such as `id` and `Unnamed: 32`.
7. Encoded the target variable, where Malignant = 1 and Benign = 0.
8. Split the dataset into 80% training and 20% testing data.
9. Standardized the feature values using StandardScaler.
10. Trained a K-Nearest Neighbors classifier with K = 5.
11. Predicted tumor classifications on the test dataset.
12. Evaluated the model using Accuracy, Precision, Recall, F1-Score, and Confusion Matrix.

## Results

The KNN model was evaluated using the following metrics:

- Accuracy: 0.956140350877193
- Precision: 0.9743589743589743
- Recall: 0.9047619047619048
- F1-Score: 0.9382716049382716

The confusion matrix is included in the Assignment-4.ipynb notebook.

## Conclusion

The K-Nearest Neighbors (KNN) algorithm was used to classify breast tumors as malignant or benign based on diagnostic measurements from the Breast Cancer Wisconsin Diagnostic Dataset. The data was preprocessed by removing unnecessary columns, encoding the target variable, and standardizing the numerical features. Standardization is particularly important for KNN because the algorithm relies on distance calculations, and features with larger numerical ranges could otherwise dominate the results. Using K = 5, the model was trained and evaluated using accuracy, precision, recall, F1-score, and a confusion matrix. The model provides a useful approach for tumor classification, but KNN has a limitation in that predictions can be computationally expensive for large datasets because it calculates distances to training samples. Its performance can also be sensitive to the choice of K and the scaling of features.
