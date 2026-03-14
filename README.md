# Diabetes Prediction using Logistic Regression

## About the Project
In this project I tried to predict whether a person has diabetes or not using a machine learning model.  
The model is built using Logistic Regression which I implemented from scratch using Python.

The dataset used for this project is the Pima Indians Diabetes dataset.

---

## Dataset Information
The dataset contains medical details of patients. Based on these features the model predicts whether the patient has diabetes.

Main columns in the dataset:

- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age
- Outcome

The **Outcome** column is the target variable:
- 0 means the person does not have diabetes
- 1 means the person has diabetes

---

## Steps I Performed

### 1. Data Loading
First I loaded the dataset using pandas and checked the first few rows to understand the data.

### 2. Checking the Data
I checked:
- missing values
- duplicate rows
- basic information of the dataset

### 3. Data Preprocessing
Some columns had 0 values which are not realistic for medical data.  
So I replaced those values with the median of the column.

### 4. Data Visualization
I plotted a graph of the Outcome column using matplotlib to see how many people have diabetes and how many do not.

### 5. Feature Selection
After checking correlation between features and the outcome, I selected these three features for my model:

- Glucose
- BMI
- Age

These features showed stronger relation with diabetes prediction.

### 6. Logistic Regression from Scratch
Instead of using sklearn, I implemented logistic regression manually using NumPy.

Steps involved:
- Initialize weights and bias
- Use sigmoid function
- Train model using gradient descent
- Run for multiple epochs

### 7. Model Evaluation
After training the model, I tested it on the test dataset and calculated the accuracy.

---

## Tools Used

- Python
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook

---

## Files in this Repository

- `diabetes.ipynb` → Jupyter notebook containing the implementation  
- `diabetes.csv` → Dataset used in the project  
- `m.doc` → Document explaining each step of the project  

---

## Conclusion
In this project I implemented a simple machine learning model to predict diabetes.  
This helped me understand how logistic regression works internally and how machine learning models are trained.
