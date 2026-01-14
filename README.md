**Aim:** To predict customer healthcare costs using the power of machine learning.  

**Dataset Summary:** insurance.csv
1. age: Age of the primary beneficiary.
2. sex: Gender of the insurance contractor (male or female).
3. bmi: Body mass index, a key indicator of body fat based on height and weight.
4. children: Number of dependents covered by the insurance plan.
5. smoker:	Indicates whether the beneficiary smokes (yes or no).
6. region:	The beneficiary's residential area in the US, divided into four regions.
7. charges: Individual medical costs billed by health insurance.

**Steps Involved:**
1. Load Data: Read insurance.csv for training and validation_dataset.csv for predictions.
2. Clean and Preprocess Training Data: Standardize categorical values (sex, smoker, region), fix invalid numeric values (age, children), and drop missing data.
3. Train Regression Model: Encode categorical features, scale numerical features, and fit a Linear Regression model; evaluate performance using cross-validation (MSE and R²).
4. Prepare Validation Data: Clean and preprocess similarly, encode categorical features, and align columns with the training dataset.
5. Predict Charges: Use the trained model to predict insurance charges for the validation dataset and add them as predicted_charges.
6. Post-process Predictions: Ensure all predicted charges are at least 1000.
