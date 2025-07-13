# Car-Price-Predictor
This is a web application built with Streamlit that predicts the price of a used car based on various input features like brand, model, fuel type, transmission, and more. It uses an XGBoost regression model trained on a labeled car dataset.

# 📁 Project Structure
📦 Car Price Predictor/
├── BrandModel.xlsx           # Mapping of brands to their models
├── ModelVariant.xlsx         # Mapping of models to their variants
├── car_dataset.csv           # Original dataset used for training
├── extracting_diffent_car_models.ipynb  # Notebook for extracting brand-model data
├── Model_Preparation_Code.ipynb         # Notebook for cleaning and model training
├── model.pkl                 # (Optional) Old XGBoost model - replaced by xgbModel.json
├── xgbModel.json             # Final trained XGBoost model
├── encoder.pkl               # Trained Target Encoder for categorical variables
├── scaler.pkl                # StandardScaler for numerical features
├── startWebApp.py            # Main Streamlit application
├── rough.py                  # Sandbox/test file
└── README.md                 # Project documentation

# ⚙️ Setup Instructions
