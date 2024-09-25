# Heart Disease Prediction using Random Forest

This project aims to predict the presence of heart disease using a Random Forest Classifier on a medical dataset. The model is trained using patient information such as age, sex, blood pressure, cholesterol levels, and other health indicators to predict whether a patient has heart disease.

## Dataset

The dataset contains 14 columns with information such as:
- Age
- Sex
- Chest pain type
- Blood pressure (BP)
- Cholesterol
- Fasting blood sugar (FBS) over 120
- Electrocardiographic (EKG) results
- Maximum heart rate (Max HR)
- Exercise-induced angina
- ST depression
- Slope of ST segment
- Number of vessels visible on fluoroscopy
- Thallium stress test results
- Heart Disease (Target variable)

The target variable `Heart Disease` has been encoded as:
- `0`: Presence of heart disease
- `1`: Absence of heart disease

## Methodology

1. **Data Preprocessing**: 
   - Loaded the dataset and checked for missing values.
   - The target variable was encoded, and features were split into `X` (input features) and `y` (target).
   
2. **Model Training**:
   - Used a Random Forest Classifier with default and tuned hyperparameters.
   - Split the data into training and test sets using an 80-20 split.

3. **Model Evaluation**:
   - Evaluated the model using accuracy, confusion matrix, and classification report.
   - Feature importance was calculated to understand the impact of each feature on the prediction.

## Hyperparameters

The following hyperparameters were used in the tuned model:

- `n_estimators=1000`
- `criterion="gini"`
- `min_samples_split=10`
- `max_depth=8`
- `random_state=5`

## Results

- The model achieved an accuracy score of ~87.
- A detailed classification report and confusion matrix can be generated to evaluate the performance.


