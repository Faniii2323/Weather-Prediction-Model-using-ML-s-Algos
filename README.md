# Weather Prediction Model

This project is a Machine Learning-based Weather Prediction System built using Python and Scikit-learn. It analyzes historical weather data and predicts the type of weather based on input features such as temperature, precipitation, and wind.

## Project Overview

The goal of this project is to:

* Predict weather conditions (e.g., rain, sun, fog)
* Compare multiple machine learning models
* Select the best-performing model based on accuracy
* Visualize model performance using confusion matrices and probability graphs

## Dataset

* **File Used:** `seattle-weather.csv`
* The dataset includes:

  * `date`
  * `precipitation`
  * `temp_max`
  * `temp_min`
  * `wind`
  * `weather` (target variable)

## Features & Processing

### 🔹 Feature Engineering

* Extracted:

  * `month` from date
  * `day` from date

### 🔹 Data Preprocessing

* Converted date column to datetime format
* Encoded weather labels using `LabelEncoder`

## Machine Learning Models Used

The following models were trained and evaluated:

* Logistic Regression
* Random Forest Classifier
* Support Vector Machine (SVM)
* K-Nearest Neighbors (KNN)
* Decision Tree Classifier

##  Model Evaluation

Each model is evaluated using:

* **Accuracy Score**
* **Confusion Matrix (printed + visualized)**

The best model is selected automatically based on highest accuracy.

## Prediction

The model allows custom input predictions using:

```python
input_data = {
    'precipitation': [10.0],
    'temp_max': [25.0],
    'temp_min': [16.0],
    'wind': [10.5],
    'month': [2],
    'day': [25]
}
```
Output:

* Predicted weather label
* Probability distribution across all weather classes

## Visualizations

* Confusion Matrix plots for each model
* Probability bar charts for predictions
* Focused comparison (e.g., Fog vs Rain)

## Technologies Used

* Python 
* NumPy
* Pandas
* Scikit-learn
* Matplotlib

## How to Run

1. Install required libraries:

```bash
pip install numpy pandas scikit-learn matplotlib
```

2. Place the dataset file in the same directory.

3. Run the notebook:

```bash
jupyter notebook "Weather Prediction Model.ipynb"
```

## Notes

* Ensure dataset path is correct.
* Label encoding must be applied before splitting data.
* Confusion matrices are meaningful when evaluating multiple samples (not single predictions).

## Future Improvements

* Improve model accuracy with hyperparameter tuning
* Add more weather features (humidity, pressure, etc.)
* Deploy as a web app using Flask or Streamlit
* Use deep learning models for better performance

## Author"FANI"

Developed as a machine learning project for understanding classification models and evaluation techniques.

---
