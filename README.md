# Heart Disease Prediction App
This project is a Streamlit-based web application that predicts the likelihood of heart disease based on user-provided health metrics. It leverages a pre-trained machine learning model and is designed to provide an easy-to-use interface for healthcare prediction tasks.

# Features
Input health parameters like age, cholesterol levels, blood pressure, etc.
Predict the likelihood of heart disease with a pre-trained machine learning model.
Simple and interactive interface powered by Streamlit.
Installation
Prerequisites
Python 3.7 or later
Required Python libraries:
pandas
streamlit
pickle
scikit-learn (if preprocessing is used)
Steps to Install
Clone the repository or download the source code:

bash
Copy code
git clone https://github.com/your-repo/heart-disease-prediction.git
cd heart-disease-prediction
Install the required dependencies:

bash
Copy code
pip install -r requirements.txt
Place your pre-trained model (heart_disease_model.pkl) and scaler (scaler.pkl, if applicable) in the project directory.

# Usage
Start the Streamlit application:

bash
Copy code
streamlit run app.py
Open your browser and navigate to:

arduino
Copy code
http://localhost:8501
Fill in the health metrics and click the Predict button to view the result.

Input Parameters
The following parameters are used to make predictions:

# Feature	Description
Age	Age of the individual (years).
Sex	Male or Female.
cp	Chest pain type (0: Typical Angina, 1: Atypical Angina, 2: Non-anginal Pain, 3: Asymptomatic).
trestbps	Resting blood pressure (mm Hg).
chol	Serum cholesterol (mg/dl).
fbs	Fasting blood sugar > 120 mg/dl (1: Yes, 0: No).
restecg	Resting electrocardiographic results (0: Normal, 1: ST-T wave abnormality, 2: Left ventricular hypertrophy).
thalach	Maximum heart rate achieved.
exang	Exercise-induced angina (1: Yes, 0: No).
oldpeak	ST depression induced by exercise relative to rest.
slope	Slope of the peak exercise ST segment (0: Upsloping, 1: Flat, 2: Downsloping).
ca	Number of major vessels (0-3) colored by fluoroscopy.
thal	Thalassemia (1: Normal, 2: Fixed Defect, 3: Reversible Defect).
How It Works
The user provides inputs for all the above parameters.
The inputs are preprocessed (e.g., scaled using a StandardScaler, if applicable).
The preprocessed data is passed to a trained machine learning model.
The app displays the prediction:
"The model predicts that this person has heart disease."
"The model predicts that this person does not have heart disease."
Files in This Project
File	Description
app.py	Main Streamlit app script.
heart_disease_model.pkl	Pre-trained machine learning model for heart disease prediction.
scaler.pkl	(Optional) Scaler object for preprocessing numeric features.
requirements.txt	List of required Python libraries.
# Example
Input:
Age: 55
Sex: Male
Chest Pain Type: Typical Angina (0)
Resting Blood Pressure: 130 mm Hg
Serum Cholesterol: 250 mg/dl
# Output:
Prediction: "The model predicts that this person does not have heart disease."
Contributing
Contributions, issues, and feature requests are welcome! Feel free to fork the repository and submit a pull request.
