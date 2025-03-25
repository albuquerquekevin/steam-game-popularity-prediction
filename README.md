# Game Popularity Prediction using Machine Learning

## Overview
This project applies machine learning techniques to predict the estimated number of game owners based on various features such as reviews, platform availability, and pricing. The dataset was sourced from Steam and preprocessed to remove irrelevant information and improve data quality.

## Dataset
The dataset consists of game-related features such as:
- Release date
- Price
- DLC count
- Platform availability (Windows, Mac, Linux)
- Positive and negative reviews
- Estimated owners (target variable)

## Data Preprocessing
Key preprocessing steps include:
- Dropping unnecessary columns
- Handling missing values
- Converting categorical variables
- Creating new features (e.g., review ratio, total reviews)
- Splitting the dataset into training and testing sets

## Model Training
The primary model used for prediction is **Random Forest Regressor**. The training pipeline includes:
1. **Feature Scaling** using `StandardScaler`
2. **Model Training** using `RandomForestRegressor`
3. **Hyperparameter Tuning** with `GridSearchCV`

## Evaluation Metrics
The model performance was assessed using:
- **Mean Squared Error (MSE)**
- **R-Squared (R²) Score**

## Feature Importance
The most influential features in predicting game popularity were analyzed using feature importance scores from the trained model. The top features contributing to predictions were visualized using `Seaborn`.

## Results
After hyperparameter tuning, the refined model achieved:
- **Refined Model Mean Squared Error:** *146308994114.553*
- **Refined Model R² Score:** *0.8440538787152014*

## Installation & Usage
```bash
# Clone the repository
git clone https://github.com/albuquerquekevin/steam-game-popularity-prediction.git

# Install dependencies
pip install -r requirements.txt

# Run the Jupyter Notebook to train the model and visualize results
jupyter notebook
```

## Future Improvements
- Experiment with additional machine learning models (e.g., Gradient Boosting)
- Enhance feature engineering techniques
- Deploy the model as an API for real-time predictions

## Repository
[GitHub Repository](https://github.com/albuquerquekevin/steam-game-popularity-prediction)

