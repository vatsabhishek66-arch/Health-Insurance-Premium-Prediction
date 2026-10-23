# Health Insurance Premium Prediction

A machine learning regression project that predicts health insurance costs based on user-provided demographic, financial, lifestyle, and medical-history information. The project includes a Streamlit web application for interactive predictions.

## Features

- Interactive web interface built with Streamlit
- Predicts estimated health insurance costs using trained machine learning models
- Uses separate models for younger users (age 25 or below) and other users
- Preprocesses categorical and numerical inputs
- Applies saved scalers to selected features
- Includes trained models and preprocessing artifacts

## Tech Stack

- Python
- Pandas
- Scikit-learn
- Joblib
- Streamlit

## Project Structure

```text
Health-Premium-Prediction/
├── app/
│   ├── main.py
│   └── prediction_helper.py
├── artifacts/
│   ├── best_model_young.joblib
│   ├── best_model_rest.joblib
│   ├── scaler_with_cols_young.joblib
│   └── scaler_with_cols_rest.joblib
├── .gitignore
├── requirements.txt
└── README.md
```

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
cd YOUR-REPOSITORY
```

Replace the repository URL with your GitHub repository URL.

### 2. Create and activate a virtual environment

Windows PowerShell:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```bash
python -m pip install -r requirements.txt
```

## Run the Application

From the project root, run:

```bash
python -m streamlit run app/main.py
```

Streamlit will display a local URL in the terminal. Open that URL in your browser to use the application.

## How It Works

1. The user enters demographic, financial, lifestyle, and medical-history details.
2. The application converts the inputs into the feature format expected by the trained models.
3. A normalized medical-risk score is calculated from the selected medical history.
4. The saved scaler transforms the required numerical features.
5. The application selects the model based on the user's age.
6. The model generates a predicted health insurance cost, which is displayed in the interface.

## Important Notes

- The prediction is an estimate from a machine learning model, not an official insurance quote.
- Prediction quality depends on the training data, feature engineering, and model performance.
- The saved model and scaler files must be available in the expected `artifacts/` directory.
- This application is intended for educational and demonstration purposes, not as a substitute for professional insurance advice.

## License

No license has been specified yet. Add a license if you intend to grant others permission to reuse or modify this project.
