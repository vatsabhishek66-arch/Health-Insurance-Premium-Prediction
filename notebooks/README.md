# Model Training Notebooks

This directory contains the Google Colab notebooks used to explore, train, and evaluate the machine learning models for the Health Insurance Premium Prediction project.

## Notebooks

1. **Overall Model Analysis** — Initial exploration and model training on the original dataset of approximately 50,000 records. This experiment helped identify the limitations of predicting premiums for younger individuals.
2. **Younger Age Group Model** — Feature engineering using genetic-risk information and training a dedicated Linear Regression model for users aged 25 or younger.
3. **Older Age Group Model** — Training and tuning a dedicated XGBoost regression model for users older than 25.

The trained models and preprocessing artifacts are used by the Streamlit application for inference.
