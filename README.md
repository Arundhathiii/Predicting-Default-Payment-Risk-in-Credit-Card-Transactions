# Credit Default Prediction Using Machine Learning

## Project Description
This project aims to predict whether a credit card user will default on their payment next month based on various features such as payment history, bill amounts, and demographic information. The machine learning pipeline is built to handle imbalanced datasets, optimize performance, and produce interpretable results suitable for real-world deployment.
The goal of this project is to develop a machine learning model that can predict the likelihood of default payment in credit card transactions, enabling financial institutions to identify high-risk customers, reduce financial losses, and improve overall risk management capabilities.

## Key Features
  * Imbalanced Data Handling: The target variable was imbalanced with a ratio of 3.52 (majority to minority). The dataset was balanced using SMOTE to achieve a ratio of 1.00.
  * Model Selection: Multiple machine learning models were tested, including Logistic Regression, Decision Tree, Random Forest, SVM, K-NN, and Gradient Boosting. Random Forest was identified as the best-performing model.
  * Hyperparameter Tuning: Grid Search Cross-Validation was applied to fine-tune the Random Forest model, evaluating 2160 parameter combinations for optimal performance.
  * Pipeline Development: A robust pipeline was created for preprocessing, oversampling, and prediction. The pipeline achieved an accuracy of 86% and an ROC-AUC score of 93.05% on the test dataset.
  * Threshold Tuning: To balance precision and recall, threshold tuning was applied to the unseen data. At a threshold of 0.4, the model achieved an accuracy of 80%, precision of 83%, and recall of 62%.

### Technologies Used
  * Python
  * Scikit-learn
  * SMOTE (imbalanced-learn)
  * Matplotlib/Seaborn for visualization

## Results
 * Best Model: Random Forest
 * Accuracy: 86% (Test Data)
 * ROC-AUC Score: 93.05%
 * Performance after Threshold Tuning (Unseen Data):
      * Accuracy: 80%
      * Precision: 83%
      * Recall: 62%
      * F1-Score: 71%
## Future Scope
  * Testing on Larger Datasets: Validate the model's performance on larger datasets.
  * Real-Time Deployment: Deploy the pipeline in a production environment for financial decision-making.
  * Dynamic Threshold Tuning: Adapt thresholding strategies for real-world cost-sensitive scenarios.
  * Incorporating Additional Features: Experiment with new features such as customer behavior metrics to further enhance predictions.
  * Explainability: Integrate SHAP or LIME for explainable AI solutions.
