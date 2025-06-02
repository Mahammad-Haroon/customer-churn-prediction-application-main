# Customer Churn Prediction Application

This project is an end-to-end machine learning solution that predicts customer churn for an e-commerce business. It includes data preprocessing, model training, evaluation, and deployment using a Flask web application.

## 📂 Project Structure

```
customer-churn-prediction-application-main/
├── churn_prediction.ipynb               # Notebook for data exploration, training, evaluation
├── data/
│   └── E_Commerce_Dataset.xlsx          # Raw dataset
├── end_to_end_deployment/
│   ├── app.py                           # Flask application for prediction
│   ├── requirements                     # Python dependencies
│   ├── Procfile                         # For Heroku deployment
│   └── env/                             # Virtual environment (optional)
```

## 🚀 Features

- **Data Preprocessing**: Handles missing values, categorical encoding, and feature scaling.
- **Modeling**: Uses machine learning models to predict customer churn.
- **Evaluation**: Performance metrics and visualizations.
- **Web App**: Flask-based web application for live predictions.
- **Deployment Ready**: Includes files for deploying to cloud platforms like Heroku.

## 📊 Dataset

The dataset `E_Commerce_Dataset.xlsx` contains anonymized records of e-commerce customer behavior used to determine churn.

## 🔧 Installation & Usage

1. **Clone the repository**:

   ```bash
   git clone https://github.com/your-username/customer-churn-prediction-application.git
   cd customer-churn-prediction-application
   ```

2. **Set up a virtual environment** (recommended):

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**:

   ```bash
   pip install -r end_to_end_deployment/requirements
   ```

4. **Run the application**:

   ```bash
   python end_to_end_deployment/app.py
   ```

   The app will be accessible at `http://127.0.0.1:5000`.

## 🌐 Deployment

To deploy the app on Heroku:

1. Install the Heroku CLI and log in.
2. From the project root:

   ```bash
   heroku create your-app-name
   git push heroku main
   ```

3. Open the deployed app:

   ```bash
   heroku open
   ```

## 📘 Notebook

Use the `churn_prediction.ipynb` notebook for:

- Data exploration
- Feature engineering
- Model training and tuning
- Saving trained models for deployment

## 📌 Notes

- The virtual environment folder (`env/`) is included in this project, but it’s generally best practice to exclude it from version control (`.gitignore`).
- Ensure the model file used in `app.py` is generated and accessible for proper inference.
