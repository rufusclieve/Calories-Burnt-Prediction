# Calories Burnt Prediction

This project is focused on predicting the number of calories burnt during physical activity using a machine learning model. The model used in this project is **XGBRegressor**, a powerful gradient boosting algorithm known for its accuracy and efficiency in regression tasks.

## Project Overview

In this project, we use a dataset containing various features related to physical exercise (such as age, gender, duration, heart rate, etc.) to predict the number of calories burnt during a session. We preprocess the data, train the model, and evaluate its performance using metrics such as **R-squared** and **Mean Absolute Error (MAE)**.

## Dataset

The dataset contains **8128 entries** and the following features:
- **Age**: The age of the individual.
- **Gender**: The gender of the individual (male/female).
- **Height**: The height of the individual (in centimeters).
- **Weight**: The weight of the individual (in kilograms).
- **Duration**: The duration of the physical activity (in minutes).
- **Heart Rate**: The heart rate during the activity (in beats per minute).
- **Body Temperature**: The body temperature during the activity (in Celsius).
- **Calories Burnt**: The target variable (calories burnt during the activity).

Missing values were handled, and the data was split into training and testing sets to evaluate the model's performance.

## Model and Techniques Used

- **XGBoost Regressor**: The primary model used for predicting the calories burnt. XGBoost is known for its efficiency and performance in machine learning tasks.
- **Feature Scaling**: Ensuring that the model performs well by normalizing the input features.
- **Train-Test Split**: The dataset was split into training and testing sets to evaluate the model.

## Results

The model's performance was evaluated using the following metrics:
- **R-squared**: 0.9988 (This indicates that the model explains 99.88% of the variance in the calories burnt.)
- **Mean Absolute Error (MAE)**: 1.483 (Given that the target variable ranges between 100 and 200, this is a good result.)

These results indicate that the model is highly accurate and performs well on unseen test data.

## Conclusion

The **XGBRegressor** performed exceptionally well on the Calories Burnt dataset, achieving a high R-squared score and a low mean absolute error. This suggests that the model is effective in predicting the number of calories burnt during physical activity. Given the MAE and the magnitude of the target variable, the results are considered strong.

## Installation

To run this project locally, you can clone the repository and install the necessary packages by running the following commands:

```bash
git clone https://github.com/your-username/calories-burnt-prediction.git
cd calories-burnt-prediction
pip install -r requirements.txt
```

## How to Use

1. **Preprocessing**: The dataset needs to be preprocessed by handling missing values and scaling the features.
2. **Model Training**: Use the XGBRegressor to train the model on the dataset.
3. **Evaluation**: After training, the model will be evaluated on the test data using metrics like R-squared and MAE.
4. **Prediction**: Use the model to predict calories burnt for new data points.
