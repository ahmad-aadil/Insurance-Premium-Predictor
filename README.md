#   Insurance Premium Category Predictor

A machine learning–powered web application that predicts **insurance premium categories**
based on user demographic, financial, and lifestyle information.

The app uses **FastAPI** as a backend REST API and **Streamlit** as an interactive frontend UI.

And describes the **data preprocessing, feature engineering, model training,
evaluation, and serialization** process used for the Insurance Premium Category Predictor.

##  Dataset Overview

The dataset contains insurance-related customer information with the following columns:

| Feature | Description |
|-------|-------------|
| age | Age of the individual |
| weight | Weight in kilograms |
| height | Height in meters |
| income_lpa | Annual income in Lakhs Per Annum |
| smoker | Smoking status (True / False) |
| city | City of residence |
| occupation | Employment category |
| insurance_premium_category | Target variable (Low / Medium / High) |


## 🛠 Feature Engineering

Several domain-driven features were created to improve model performance.


##  Features

- Predicts insurance premium category
- Displays confidence score
- Shows class-wise probability

##  Tech Stack

**Backend**
- FastAPI
- Uvicorn
- Scikit-learn
- Pandas
- NumPy

**Frontend**
- Streamlit
- Requests

**Sample Input**
{
  "age": 30,
  "weight": 65,
  "height": 1.7,
  "income_lpa": 10,
  "smoker": true,
  "city": "Mumbai",
  "occupation": "retired"
}


**Sample Output**
{
  "predicted_category": "Medium",
  "confidence": 0.92,
  "class_probabilities": {
    "Low": 0.05,
    "Medium": 0.92,
    "High": 0.03
  }
}


Author

Aadil Ahmad
