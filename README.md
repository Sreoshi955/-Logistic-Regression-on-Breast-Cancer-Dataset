Logistic Regression on Breast Cancer Dataset

This project applies a Logistic Regression model to a binary classification problem using the Breast Cancer Wisconsin Diagnostic Dataset. The goal is to classify whether a tumor is malignant (M) or benign (B) based on various features extracted from medical imaging.

Dataset

The dataset contains 569 samples with 30 numerical features and a target variable diagnosis:

* M → Malignant
* B → Benign

Unnecessary columns like id and Unnamed: 32 are removed, and the target is mapped to binary (M=1, B=0).

Workflow

1. Data Preprocessing

* Loaded dataset from CSV
* Dropped irrelevant columns
* Mapped labels to binary
* Checked dataset info and structure

2. Train-Test Split & Feature Scaling

* Split into 80% training and 20% testing
* Standardized all features using StandardScaler

3. Model Training

* Trained a Logistic Regression model using scikit-learn
* Evaluated on test set

4. Evaluation Metrics

* Confusion Matrix
* **Classification Report** (Precision, Recall, F1-Score)
* ROC-AUC Score: 0.997
* ROC Curve plotted

5. Threshold Tuning

* Tested thresholds: 0.4, 0.5, 0.6
* Compared Precision, Recall, and F1-Score for each threshold
* Explained the Sigmoid Function used in Logistic Regression

Results

  Threshold   Precision    Recall    F1 Score 
  0.4         0.9767      0.9767     0.9767   
  0.5         0.9762      0.9535     0.9647   
  0.6         1.0000      0.9535     0.9762   

ROC-AUC Score

* ROC-AUC: 0.997 → excellent classifier performance.

Technologies Used

* Python
* Pandas, NumPy
* scikit-learn
* Matplotlib (for ROC curve)

Concepts Covered

* Binary classification
* Logistic regression
* Feature scaling
* Model evaluation metrics
* Threshold tuning
* Sigmoid activation
