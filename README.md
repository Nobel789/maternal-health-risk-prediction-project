# Maternal Health Risk Prediction

This repository contains a machine learning portfolio project for predicting **maternal health risk level** using clinical health measurements.

The project uses a tabular maternal health dataset and a saved machine learning model to classify risk level.

## Project Goal

The goal of this project is to build a machine learning workflow that predicts maternal health risk based on health-related features such as age, blood pressure, blood sugar, body temperature, and heart rate.

This project is for learning and portfolio demonstration only. It is **not** a medical diagnostic tool.

## Repository Files

Your uploaded repository currently contains:

```text
maternal-health-risk-prediction-project/
├── README.md
├── .gitignore
├── requirements.txt
├── LICENSE
├── Data_README.md
├── maternal_health_risk_prediction.ipynb
├── Maternal_Health_Risk_Data_Set_Modified.csv
└── risk_model.joblib
```

## Main Notebook

### `maternal_health_risk_prediction.ipynb`

This notebook includes the full machine learning workflow:

- Loading the maternal health risk dataset
- Exploring the data
- Checking missing values
- Cleaning and preparing the target labels
- Splitting data into training and testing sets
- Training a machine learning model
- Evaluating model performance
- Saving or loading the trained model

## Dataset

The dataset file is:

```text
Maternal_Health_Risk_Data_Set_Modified.csv
```

The target column is usually:

```text
RiskLevel
```

The project predicts maternal risk categories such as:

```text
low risk
high risk
```

Depending on the dataset version, labels may have different capitalization, such as `Low risk` or `HIGH risk`. These should be cleaned before training so the model learns consistent classes.

## Saved Model

The saved model file is:

```text
risk_model.joblib
```

You can load it using:

```python
import joblib

model = joblib.load("risk_model.joblib")
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

### 4. Open the Notebook

```bash
jupyter notebook
```

Then open:

```text
maternal_health_risk_prediction.ipynb
```

Run the notebook cells from top to bottom.

## Example Project Workflow

The project follows this general workflow:

```text
Load dataset
↓
Explore and clean data
↓
Prepare features and target
↓
Train machine learning model
↓
Evaluate model performance
↓
Save trained model
↓
Use saved model for prediction
```

## Important Medical Disclaimer

This project is for education and portfolio demonstration only.

It should **not** be used for real diagnosis, treatment, triage, or clinical decision-making. Any real healthcare machine learning system requires clinical validation, expert medical review, privacy review, and regulatory approval.

## Skills Demonstrated

This project demonstrates:

- Healthcare data analysis
- Data cleaning
- Feature and target preparation
- Classification modeling
- Model evaluation
- Saving and loading trained models
- Jupyter Notebook organization
- GitHub portfolio documentation

## Future Improvements

Possible next steps:

- Add confusion matrix visualization
- Add classification report results to this README
- Compare multiple models
- Add feature importance analysis
- Add example predictions
- Build a small Streamlit web app
- Improve label cleaning for `RiskLevel`
- Add model performance screenshots

## Author

Created by **Nobel789** as a healthcare AI and machine learning portfolio project.

## License

This project is licensed under the MIT License.
