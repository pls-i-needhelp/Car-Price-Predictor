# Car Price Predictor Project

This repository contains a machine learning project designed to predict the price of used cars based on various features. The project includes data preprocessing, model training, and a web application for user interaction.

## Project Structure

- `BrandModel.xlsx`: Excel file containing car brands and models.
- `ModelVariant.xlsx`: Excel file containing car models and their variants.
- `car_dataset.csv`: Dataset with car details including price, mileage, etc.
- `extracting_different_car_models.ipynb`: Jupyter notebook for initial data exploration and extraction.
- `Model_Preparation_Code.ipynb`: Jupyter notebook for data preprocessing, feature engineering, and model training.
- `ModelVariant`: CSV file with model variants.
- `startWebApp.py`: Python script for the Streamlit web application.
- `model.pkl`, `encoder.pkl`, `scaler.pkl`: Pickle files containing the trained model, target encoder, and scaler.
- `scaler.pkl`, `encoder.pkl`: Pickle files for preprocessing transformations.
- `xgModel`: Additional model-related file.

## Setup Instructions

1. **Install Dependencies**:
   Ensure you have Python installed. Install the required libraries using the following command:
   ```bash
   pip install pandas numpy streamlit openpyxl category_encoders sklearn xgboost
   ```

2. **Prepare the Environment**:
   - Place all `.xlsx`, `.csv`, and `.pkl` files in the project directory.
   - Ensure the Jupyter notebooks are accessible for review or execution.

3. **Run the Web Application**:
   - Navigate to the project directory in your terminal.
   - Run the web app using:
     ```bash
     streamlit run startWebApp.py
     ```
   - Open your browser and go to the provided local URL (usually `http://localhost:8501`) to use the car price predictor.

## Usage

- The web application allows users to input car details such as brand, model, variant, year, fuel type, seller type, transmission, owner type, mileage, kilometers driven, seating capacity, and engine power.
- Click the "Predict" button to get an estimated price based on the trained model.

## Model Training

- The `Model_Preparation_Code.ipynb` notebook contains the complete workflow for training the model:
  - Data loading and exploration.
  - Feature engineering and preprocessing.
  - Training and evaluation of multiple regression models (e.g., XGBoost, LightGBM, KNN, SVR).
  - Model selection and final training on the full dataset.
- The best model (XGBoost) is saved as `model.pkl` along with the `scaler.pkl` and `encoder.pkl` for preprocessing.

## Contributing

Feel free to fork this repository, make improvements, and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
