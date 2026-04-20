# KNN Classification Analysis

## Overview

This project applies the **K-Nearest Neighbors (KNN)** algorithm to two datasets:

* `KNN_Project_Data`
* `Classified Data`

The goal is to build a classification model, evaluate its performance, and improve results by tuning the number of neighbors (**K**).

---

## Methodology

The following steps were applied to both datasets:

1. **Data Loading**

   * Imported datasets using pandas

2. **Exploratory Data Analysis (EDA)**

   * Pairplot visualization (for KNN_Project_Data)

3. **Feature Scaling**

   * Applied `StandardScaler` to normalize all features
   * Necessary for distance-based models like KNN

4. **Train-Test Split**

   * Split data into training and testing sets (70/30)

5. **Model Training**

   * Trained a KNN classifier with `k = 1`

6. **Evaluation**

   * Used:

     * Confusion Matrix
     * Classification Report

7. **Hyperparameter Tuning**

   * Used the elbow method to test values of K (1–39)
   * Selected optimal K based on lowest error rate

8. **Retraining**

   * Re-trained the model using the optimal K value
   * Compared performance before and after tuning

---

## Results

* Performance improved after tuning K, showing reduced overfitting compared to `k = 1`
* The model achieved higher accuracy and more balanced precision/recall

---

## Key Insights

* KNN performance is highly dependent on feature scaling
* Smaller K values can lead to overfitting
* Larger K values improve generalization but may smooth decision boundaries

---

## Technologies Used

* Python
* pandas
* NumPy
* scikit-learn
* seaborn
* matplotlib

---

## Author
Fatimah Al-Maqhawi
