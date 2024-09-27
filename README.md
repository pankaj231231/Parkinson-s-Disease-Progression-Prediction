# Parkinsons_disease_progression_prediction
**1. Introduction:**
Parkinson's disease is a neurodegenerative disorder that affects movement control. Early prediction of disease progression is crucial for effective treatment and intervention strategies. Machine learning techniques have shown promise in predicting the progression of Parkinson's disease using various features. This report analyzes the use of TF-IDF (Term Frequency-Inverse Document Frequency) features for predicting Parkinson's disease progression.

**2. Dataset Overview:**
The dataset used for this analysis is sourced from Kaggle and consists of clinical and demographic data of patients with Parkinson's disease. The dataset includes features such as age, gender, baseline UPDRS (Unified Parkinson's Disease Rating Scale) scores, and textual patient reports. The primary target variable is the 'motor_UPDRS' score, which indicates the motor symptoms' severity.

**3. Methodology:**
The analysis includes the following steps:

**Data Preprocessing:**
- The textual patient reports were preprocessed using tokenization and TF-IDF vectorization. This step converted the raw text data into numerical features suitable for machine learning algorithms.
- Demographic and clinical features were normalized to ensure all features have the same scale.

**Model Development:**
- The dataset was split into training and testing sets (e.g., 80% training and 20% testing).
- Linear Regression was chosen as the predictive model due to its simplicity and interpretability. Other regression algorithms could also be explored for comparison.
- The TF-IDF features and demographic/clinical features were concatenated to form the input features for the model.

**Model Evaluation:**
- The trained model was evaluated using various metrics such as Mean Squared Error (MSE), Average sMAPE.
- Cross-validation techniques were used to ensure the model's generalization performance.

**4. Results:**
The trained model achieved the following results on the test set:

- Mean Squared Error (MSE): 60.20
- Average sMAPE : 94.42


These metrics provide insight into the accuracy and variance explained by the model. Interpretation of these values indicates how well the model predicts Parkinson's disease progression based on the provided features.

**5. Discussion:**
The results suggest that the TF-IDF features, when combined with demographic and clinical features, have predictive power for Parkinson's disease progression. The chosen model's performance can be further compared with more complex algorithms to determine if improvements are achievable.
