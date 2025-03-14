# Heart-Disease-Prediction
Developing a predictive model capable of accurately identifying individuals with heart disease

This project aims to predict the likelihood of heart disease using Decision Tree (DT), K-Nearest Neighbors (KNN), and Support Vector Machine (SVM). The pipeline includes data exploration, preprocessing, model training, hyperparameter tuning, evaluation, and comparison to determine the best model for this classification problem.

## Summary Statistics and Initial Data Exploration
Loaded the dataset and examined its structure.
Computed summary statistics, including mean, median, standard deviation, and missing values.
Checked the distribution of numerical features to identify skewness and outliers.
<img width="1146" alt="Screen Shot 2025-03-14 at 10 57 04 AM" src="https://github.com/user-attachments/assets/12ce1c02-4dbd-473d-aefb-503b6d8a5342" />

## Exploratory Data Analysis (EDA)
Visualized feature distributions using histograms and KDE plots.
Analyzed feature correlations using a heatmap to identify relationships between variables.
Checked class imbalance to understand whether data balancing techniques were needed.

## Data Preprocessing
Handled missing values if any were present.
Performed feature transformation:
Applied Box-Cox transformation to reduce skewness in numerical features.
Standardized features for KNN and SVM, as they are sensitive to feature scales.
Split the dataset into training (X_train_set, y_train_set) and test sets (X_test_set, y_test_set) for model evaluation.

## Model Training and Hyperparameter Tuning
We implemented three models with optimized hyperparameters using Grid Search with Cross-Validation.

## Decision Tree (DT)
Defined a baseline DT model.
Tuned hyperparameters
<img width="1146" alt="Screen Shot 2025-03-14 at 10 57 41 AM" src="https://github.com/user-attachments/assets/ac6508de-a6af-4993-ab4e-44d91dd3204e" />

## K-Nearest Neighbors (KNN)
<img width="1046" alt="Screen Shot 2025-03-14 at 10 57 59 AM" src="https://github.com/user-attachments/assets/06aff254-d9f1-4830-b8d4-226c578f0ea5" />

## Support Vector Machine (SVM)
<img width="1046" alt="Screen Shot 2025-03-14 at 10 58 11 AM" src="https://github.com/user-attachments/assets/2936121a-ece3-457e-882b-90aeac8c14dc" />

## Model Evaluation and Comparison

SVM achieved the highest recall (1.00), meaning it successfully identified all positive cases, which is crucial in medical applications where missing a diagnosis could have serious consequences.
KNN had the highest accuracy (0.84), showing balanced precision and recall across both classes.
Decision Tree performed well overall, offering a good balance of precision, recall, and explainability.
<img width="1046" alt="Screen Shot 2025-03-14 at 10 58 34 AM" src="https://github.com/user-attachments/assets/1f6e9d75-3cfa-40e4-be95-ae5723647771" />

## Key Takeaways & Conclusion
If recall is the top priority (e.g., detecting all heart disease cases), SVM is the best choice.
If balanced performance with high accuracy is desired, KNN is the best option.
If interpretability is required, Decision Tree is a suitable choice.

