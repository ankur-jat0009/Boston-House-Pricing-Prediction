# House Price Prediction Using Machine Learning

## Project Overview
This project aims to predict house prices based on various features using a **Linear Regression model** trained on the **Boston Housing Dataset**. The trained model is deployed using **Flask**, providing both a web-based interface and an API for real-time predictions.

## Tech Stack
- **Programming Language:** Python
- **Libraries:** Scikit-Learn, Pandas, NumPy, Matplotlib, Seaborn
- **Framework:** Flask
- **Model Storage:** Pickle
- **Frontend:** HTML

## Features
- **Data Preprocessing:** Handles missing values, performs feature scaling, and explores feature correlations.
- **Model Training:** Uses **Linear Regression** and evaluates performance using **Mean Squared Error (MSE)** and **R-squared (R²) score**.
- **Web Interface:** A simple **Flask-based web app** where users can input house details and get price predictions.
- **API Endpoint (`/predict_api`)**: Accepts JSON data and returns predictions.
- **Model Deployment:** Saves the trained model using **Pickle** for quick and efficient loading.

## Installation & Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/ankur-jat0009/house-price-prediction.git
   cd house-price-prediction
   ```
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Flask application:
   ```bash
   python app.py
   ```
4. Open the web app in your browser:
   ```
   http://127.0.0.1:5000/
   ```

## API Usage
- **Endpoint:** `POST /predict_api`
- **Request Format (JSON):**
   ```json
   {
     "CRIM": 0.1,
     "ZN": 25.0,
     "INDUS": 5.0,
     "RM": 6.5,
     "AGE": 40.0,
     "DIS": 4.0,
     "RAD": 1.0,
     "TAX": 300.0,
     "PTRATIO": 15.0,
     "B": 396.0,
     "LSTAT": 5.0
   }
   ```
- **Response:**
   ```json
   {
     "predicted_price": 22.5
   }
   ```

### Software And Tools Requirements

1. [Github Account](https://github.com)
3. [VSCodeIDE](https://code.visualstudio.com/)
4. [GitCLI](https://git-scm.com/book/en/v2/Getting-Started-The-Command-Line)

Create a new environment

```
conda create -p venv python==3.7 -y
```
