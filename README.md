# Obesity Level Classification & Behavioral Analytics

## 🎯 Overview
This project focuses on predicting individual obesity levels—ranging from **Insufficient Weight** to **Obesity Type III**—using lifestyle, dietary, and demographic factors. By leveraging supervised machine learning, this study provides an evidence-based tool for the early identification of individuals at health risk, supporting preventive healthcare and personalized lifestyle interventions.

## 📊 Dataset & Preprocessing
* **Source:** UCI Machine Learning Repository (2,111 samples, 17 features).
* **Numerical Features:** Features such as Age, Weight, and Height were standardized using **Z-score normalization** to ensure model compatibility.
* **Categorical Features:** Multi-level variables (e.g., Transportation Mode, Alcohol Consumption) were converted via **one-hot encoding**.
* **Data Split:** The dataset was partitioned into an **80% training set** and a **20% testing set** using stratified sampling.



## 🛠️ Machine Learning Modeling
I compared five supervised learning algorithms to identify the most robust classifier:
1. **Logistic Regression with Lasso:** Used L1 regularization to reduce overfitting and select key predictors.
2. **Support Vector Machines (SVM):** Optimized with a linear kernel and cost parameter tuning ($Cost=100$).
3. **K-Nearest Neighbors (KNN):** Evaluated across various $k$ values, with $k=1$ providing the best performance.
4. **Decision Trees:** Used to visualize the hierarchical structure of health-related decision-making.
5. **Linear Discriminant Analysis (LDA):** Employed as a stable baseline linear classifier.

## 🏆 Key Results
The **Lasso-regularized model** was selected as the optimal choice due to its high accuracy and stability:
* **Test Accuracy:** **96.43%**[cite: 1112, 1262].
* **Mean Squared Error (MSE):** **0.2214**, the lowest among all candidates.
* **Feature Importance:** **Weight**, **Height**, and **Vegetable Consumption (FCVC)** were identified as the most significant predictors for obesity classification.



## 🚀 Technologies Used
* **Language:** R (for EDA, visualization, and advanced statistical modeling).
* **Libraries:** `glmnet` (Lasso), `e1071` (SVM), `rpart` (Decision Tree), `caret` (Cross-validation), `ggplot2` (Data Visualization).

## 👥 Authors
* Dongni Li
* Meng Hsuan Ho
* Pin Tzu Tseng
