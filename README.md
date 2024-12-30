# Real Estate Price Prediction

## Overview
This project aims to predict real estate prices using machine learning models in Python. By leveraging data science techniques, the project explores how factors like house age, proximity to MRT stations, number of convenience stores, and geographical coordinates influence housing prices. Two models, Random Forest Regressor and Linear Regression, were built, evaluated, and compared.

## Features
- Data preprocessing and cleaning.
- Exploratory Data Analysis (EDA) to uncover insights.
- Model training using Random Forest Regressor and Linear Regression.
- Model evaluation using metrics like Root Mean Squared Error (RMSE) and R-squared (R²).
- Prediction functionality for new property data.

## Tools and Libraries Used
- **Python**: Core programming language.
- **Pandas & NumPy**: Data manipulation and analysis.
- **Matplotlib & Seaborn**: Data visualization.
- **Scikit-learn**: Machine learning algorithms and evaluation metrics.

## Project Workflow
1. **Data Loading and Exploration**:  
   - The dataset contains features like `Transaction Date`, `House Age`, `Distance to MRT Station`, `Number of Convenience Stores`, `Latitude`, `Longitude`, and `House Price of Unit Area`.
   - Shape of the dataset: 414 rows, 7 columns.

2. **Data Preprocessing**:  
   - Handled missing values by replacing them with column means.
   - Normalized features using `StandardScaler`.

3. **Model Development**:  
   - **Random Forest Regressor**: Used 100 estimators with a random state of 42.
   - **Linear Regression**: Built as a baseline model.

4. **Evaluation Metrics**:  
   - Root Mean Squared Error (RMSE).  
   - R-squared (R²) score.

5. **Prediction Function**:  
   - Created a function to predict house prices based on user-provided inputs.

## Results
### Model Performance:
- **Random Forest Regressor**:  
  - RMSE: $6.32  
  - R² Score: 0.8557
- **Linear Regression**:  
  - RMSE: $13.49  
  - R² Score: 0.3422

### Example Prediction:
For a sample house with the following details:
- House age: 10 years
- Distance to MRT station: 500 meters
- Number of convenience stores: 5
- Latitude: 25.03
- Longitude: 121.53

The predictions were:
- **Random Forest Predicted Price**: $35.96 per unit area.
- **Linear Regression Predicted Price**: $2,117.12 per unit area.

## How to Run
1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```

2. Install required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter Notebook or Python script to execute the project.

4. Modify the `sample_house` dictionary in the script to predict prices for custom data.

## Conclusion
This project demonstrates the practical application of machine learning in the real estate domain, providing actionable insights and accurate predictions for property pricing. It highlights the efficiency of Random Forest over Linear Regression for this dataset.

## Future Work
- Experiment with additional machine learning models.
- Implement hyperparameter tuning for Random Forest.
- Explore deep learning techniques for improved performance.
