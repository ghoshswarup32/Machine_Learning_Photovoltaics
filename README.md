# Machine_Learning_Photovoltaics
Contains data of Janus materials with machine learning models
# Photovoltaic Efficiency Prediction Pipeline

This repository implements a **machine learning and deep learning pipeline** for predicting the photovoltaic (PV) efficiency of Janus materials. The workflow integrates **data screening, classification, regression, deep learning, and stacked ensemble modeling**.

---

## 📌 Workflow Steps

1. **Data Screening**
   - Load dataset (`your_dataset.csv`).
   - Keep only materials with bandgap `Eg > 0`.
   - Label compounds as PV if `1.0 ≤ Eg ≤ 2.5`.

2. **Classification**
   - Train classifiers (e.g., Random Forest).
   - Identify potential PV candidates.
   - Evaluate with **Confusion Matrix, F1 Score, ROC-AUC**.

3. **Feature Selection**
   - Select features: `Eg, n_ph, FF, P_max`.

4. **Regression Models**
   - Random Forest Regressor (RFR)  
   - Support Vector Regression (SVR)  
   - Kernel Ridge Regression (KRR)  
   - XGBoost Regressor  (XGBoost)
   - Symbolic Regression (SR)

5. **Deep Learning Models**
   - **ANN**: Multi-layer fully connected network.  
   - **CNN**: 1D convolutional layers.  
   - **RNN**: LSTM-based network.
   - **DNN**: Deep neural netwoek.
   - **MPNN**: Message Passing.  

6. **Stacked Model**
   - Base learners: ML + DL models.  
   - Meta learner: CNN+KRR.  
   - Produces final predictions.

7. **Evaluation Metrics**
   - Mean Absolute Error (MAE)  
   - Root Mean Square Error (RMSE)  
   - R² Score  

8. **Outputs**
   - Saved models (`.joblib`, `.h5`).  
   - Metrics and plots for comparison.  

---

## 🗂 Repository Structure

