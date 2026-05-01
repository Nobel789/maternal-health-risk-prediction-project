# Maternal Health Risk Prediction

This repository contains a machine learning portfolio project for predicting **maternal health risk level** using patient health measurements.

The project uses a tabular dataset and a trained machine learning model to classify maternal health risk into categories such as low, mid, or high risk.

## Project Goal

The goal of this project is to build a machine learning workflow that can predict maternal health risk level from clinical features.

This project is for learning and portfolio demonstration only. It is **not** a medical diagnostic tool.

## Repository Files

```text
maternal-health-risk-prediction-project/
├── README.md
├── .gitignore
├── requirements.txt
├── LICENSE
├── Data_README.md
├── maternal_health_risk_prediction.ipynb
├── data/
│   └── Maternal_Health_Risk_Data_Set_Modified.csv
└── models/
    └── risk_model.joblib
```

## Main Notebook

### `maternal_health_risk_prediction.ipynb`

The notebook includes:

- Loading the maternal health risk dataset
- Exploring dataset features
- Checking missing values
- Visualizing feature relationships
- Preparing features and target labels
- Training machine learning models
- Evaluating model performance
- Saving or loading the trained model

## Dataset

The dataset included in this project is:

```text
data/Maternal_Health_Risk_Data_Set_Modified.csv
```

Dataset summary:

```text
Dataset rows: 679
Dataset columns: 8
Target column: RiskLevel
Class distribution: {'low risk': 404, 'high risk': 271, 'Low risk': 3, 'HIGH risk': 1}
```

Main columns:

- `CitizenID`
- `Age`
- `SystolicBP`
- `DiastolicBP`
- `BS`
- `BodyTemp`
- `HeartRate`
- `RiskLevel`

## Saved Model

The saved model file is:

```text
models/risk_model.joblib
```

This file can be loaded with `joblib` if you want to reuse the trained model.

Example:

```python
import joblib

model = joblib.load("models/risk_model.joblib")
```

## Tools and Libraries

This project uses:

- Python
- pandas
- NumPy
- scikit-learn
- Matplotlib
- Seaborn
- Joblib
- Jupyter Notebook

## How to Run This Project

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/maternal-health-risk-prediction-project.git
cd maternal-health-risk-prediction-project
```

Replace `YOUR-USERNAME` with your GitHub username.

### 2. Create a Virtual Environment

For Windows:

```bash
python -m venv venv
venv\Scripts\activate
```

For macOS or Linux:

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Required Libraries

```bash
pip install -r requirements.txt
```

### 4. Open Jupyter Notebook

```bash
jupyter notebook
```

Then open:

```text
maternal_health_risk_prediction.ipynb
```

Run the notebook cells from top to bottom.

## Important Medical Disclaimer

This project is for education and portfolio demonstration only.

It should not be used for real diagnosis, treatment, triage, or clinical decision-making. Any real healthcare machine learning model requires clinical validation, privacy review, regulatory review, and expert medical oversight.

## Skills Demonstrated

This project demonstrates:

- Healthcare data analysis
- Data cleaning and preprocessing
- Classification modeling
- Model evaluation
- Saving and loading machine learning models
- Jupyter Notebook project organization
- GitHub portfolio documentation

## Future Improvements

Possible next steps:

- Add confusion matrix visualization
- Add classification report summary to the README
- Compare multiple models side by side
- Add feature importance analysis
- Add a Streamlit web app demo
- Add model prediction examples
- Improve notebook explanations for beginners

## Author

Created by **Nobel789** as a healthcare AI and machine learning portfolio project.

## License

This project is licensed under the MIT License.
