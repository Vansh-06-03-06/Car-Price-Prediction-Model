# Car Price Predictor

This is a machine learning project that predicts the price of a car based on features like its make, model, year, and fuel type. The web application is built using **Flask**.

## Features
- Fully functional web interface with dropdowns populated dynamically from the dataset.
- Uses `scikit-learn`'s `LinearRegression` pipeline with `OneHotEncoder` and `ColumnTransformer`.
- Fast, local, and deployable.

## How to Run Locally

1. Make sure Python is installed on your computer.
2. Install the necessary dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Flask application:
   ```bash
   python application.py
   ```
4. Open your web browser and go to `http://127.0.0.1:5000/`.

## Deployment
This project is configured to be deployed easily on platforms like **Render.com** or **PythonAnywhere**.
- `gunicorn` is included in `requirements.txt` for production-grade web serving.
- Start command for Render: `gunicorn application:app`

## Files Included
- `application.py`: The main Flask server script.
- `Car_Predictor.ipynb`: The Jupyter Notebook used for data cleaning and training the Linear Regression model.
- `LinearRegressionModel.pkl`: The trained model exported via Pickle.
- `Cleaned Car.csv`: The cleaned dataset used by the web app for its dropdowns.
- `templates/` & `static/`: HTML, CSS, and JS for the web interface.
