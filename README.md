# GlucoPredict — Diabetes Risk Prediction System

GlucoPredict is a machine learning-based project that predicts diabetes using patient health-related attributes. The project covers the complete basic workflow from loading and preparing the dataset to model training and evaluation.

## Overview

The model uses health-related attributes such as glucose level, blood pressure, BMI, age, and other available patient information to predict whether a patient record indicates diabetes.

The project is implemented in Python using Pandas, NumPy, Matplotlib, Seaborn, and Scikit-learn.

## Features

* Load and analyze diabetes patient data
* Data preprocessing
* Exploratory Data Analysis (EDA)
* Data visualization
* Machine learning model development
* Model training
* Model evaluation
* Diabetes prediction for new patient data

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Machine Learning

## Dataset

The project uses a diabetes dataset containing patient health-related attributes, including glucose level, blood pressure, BMI, age, and other medical attributes.

The dataset is included in the repository as:

```text
diabetes.csv
```

## Project Structure

```text
GlucoPredict-Diabetes-Risk-Prediction-System/
│
├── Diabetes_Prediction_Model.py
├── diabetes.csv
└── README.md
```

The main Python script contains the data preprocessing, model building, training, and evaluation workflow.

# Setup and Usage

## 1. Prerequisites

Make sure the following are installed:

* Python 3.x
* pip
* Git

You can verify Python and pip installation with:

```bash
python --version
pip --version
```

## 2. Clone the Repository

Clone the project repository and move into the project directory:

```bash
git clone <repository-url>
cd GlucoPredict-Diabetes-Risk-Prediction-System
```

## 3. Create a Virtual Environment

Creating a virtual environment keeps the project's dependencies isolated.

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### macOS / Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

After activation, your terminal should show the virtual environment name.

## 4. Install Dependencies

Install the required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

You can verify the installation with:

```bash
pip list
```

## 5. Verify the Dataset

Make sure `diabetes.csv` is located in the same project directory as the Python script:

```text
GlucoPredict-Diabetes-Risk-Prediction-System/
│
├── Diabetes_Prediction_Model.py
├── diabetes.csv
└── README.md
```

The current repository contains these three files.

## 6. Run the Project

Execute the main Python script:

```bash
python Diabetes_Prediction_Model.py
```

The script performs the project workflow, including:

```text
Load Dataset
     ↓
Data Preprocessing
     ↓
Exploratory Data Analysis
     ↓
Prepare Data
     ↓
Build Machine Learning Model
     ↓
Train Model
     ↓
Evaluate Model
     ↓
Generate Prediction
```

The repository documentation describes the script as handling preprocessing, model building, training, and evaluation.

## 7. Sample Prediction Usage

After the model has been trained, a new patient record can be passed to the trained model using the same feature format used during training.

Example:

```python
sample_patient = [[6, 148, 72, 35, 0, 33.6, 0.627, 50]]

prediction = model.predict(sample_patient)

if prediction[0] == 1:
    print("Diabetes predicted")
else:
    print("No diabetes predicted")
```

### Sample Input

```text
Pregnancies: 6
Glucose: 148
Blood Pressure: 72
Skin Thickness: 35
Insulin: 0
BMI: 33.6
Diabetes Pedigree Function: 0.627
Age: 50
```

### Sample Output

```text
Diabetes predicted
```

> This example demonstrates how a trained model can be used for prediction. The feature order and preprocessing must match the model's training pipeline.

## 8. Complete Execution Flow

For a fresh setup, follow these steps in order:

```bash
# Clone the repository
git clone <repository-url>

# Enter the project
cd GlucoPredict-Diabetes-Risk-Prediction-System

# Create virtual environment
python -m venv venv

# Activate environment - Windows
venv\Scripts\activate

# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn

# Run the project
python Diabetes_Prediction_Model.py
```

The dataset should already be available as `diabetes.csv` in the project directory.

## Skills Demonstrated

* Python Programming
* Data Preprocessing
* Exploratory Data Analysis
* Data Visualization
* Machine Learning
* Classification
* Model Training
* Model Evaluation
* Pandas
* NumPy
* Scikit-learn

## Learning Outcomes

This project provides practical experience with a complete machine learning workflow:

* Preparing a real-world-style dataset
* Exploring relationships between health-related variables
* Visualizing data
* Preparing features for machine learning
* Training a classification model
* Evaluating model performance
* Using a trained model to generate predictions

## Disclaimer

This project is intended for educational and portfolio purposes. It is not a medical diagnostic system and should not be used as a substitute for professional medical advice or diagnosis.

## Author

**Anil Jadhav**
