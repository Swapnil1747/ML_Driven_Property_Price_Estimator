# Housing Price Prediction with Multiple Regression Models and Flask GUI

This project is a web application for predicting housing prices using multiple regression models. It features a Flask-based graphical user interface (GUI) that allows users to input housing data and get price predictions from various machine learning models. The project also includes model evaluation results for comparison.

## Features

- Predict housing prices using 13 different regression models:
  - Linear Regression
  - Robust Regression (Huber Regressor)
  - Ridge Regression
  - Lasso Regression
  - ElasticNet
  - Polynomial Regression
  - Stochastic Gradient Descent Regressor (SGDRegressor)
  - Artificial Neural Network (ANN)
  - Random Forest Regressor
  - Support Vector Machine (SVM)
  - LightGBM Regressor
  - XGBoost Regressor
  - K-Nearest Neighbors (KNN)

- View model evaluation results including MAE, MSE, and R2 scores.
- User-friendly web interface for inputting housing features and viewing predictions.

## Installation

1. Clone the repository or download the project files.

2. Ensure you have Python 3.7 or higher installed.

3. It is recommended to create a virtual environment:

```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

4. Install the required Python packages:

```bash
pip install -r requirements.txt
```

## Usage

1. Run the Flask application:

```bash
python app.py
```

2. Open your web browser and navigate to:

```
http://127.0.0.1:5000/
```

3. Select a regression model, enter the housing features, and submit to get the predicted price.

4. You can also view the model evaluation results by navigating to the "Results" page.

## Project Structure

- `app.py`: Main Flask application that serves the web interface and handles predictions.
- `model.py`: Script to train the regression models, save them as pickle files, and generate evaluation results.
- `*.pkl`: Pickle files containing the trained models.
- `model_evaluation_results.csv`: CSV file containing evaluation metrics for each model.
- `templates/`: HTML templates for the web pages.
- `static/`: Static files such as CSS stylesheets.

## Dataset

The models are trained on the USA Housing dataset (`USA_Housing.csv`), which includes features such as average area income, house age, number of rooms, bedrooms, and area population.

## License

This project is provided as-is for educational and demonstration purposes.
