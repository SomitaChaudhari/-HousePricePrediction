# HousePricePrediction
This is a house price prediction system that helps users predict house prices based on locality, number of of bedrooms, bathrooms and total sqft area.  This project provides an advanced machine learning-based solution to predict house prices in the Bengaluru real estate market. It leverages robust data cleaning, feature engineering, and a state-of-the-art Ridge Regression model, all integrated within an interactive Flask web application for real-time predictions. The goal of this project is to deliver accurate and actionable house price predictions. By combining a thorough data processing pipeline, a finely-tuned predictive model, and a user-friendly interface, the system offers valuable insights for stakeholders in the real estate market.

## Dataset

- **Source:** Real-world housing data from Bengaluru.
- **Raw Data:** `Bengaluru_House_Data.csv` (initial dataset).
- **Cleaned Data:** `Cleaned_data.csv`, which includes:
  - **Location:** Categorical variable indicating the neighborhood.
  - **Total Square Footage:** Numerical value representing the property size.
  - **BHK:** Number of bedrooms.
  - **Bathrooms:** Number of bathrooms.
  - **Price:** The target variable for prediction.
- **Preprocessing:** Data cleaning involved outlier removal, handling missing values, and normalization to ensure high data quality.

## Methodology

1. **Data Preprocessing:**  
   - Comprehensive cleaning and normalization of the raw dataset.
   - Encoding of categorical features (e.g., location) to prepare for modeling.
   
2. **Feature Engineering:**  
   - Derivation of new features to capture complex property relationships.
   - Selection of the most impactful predictors through statistical analysis.
   
3. **Model Selection & Training:**  
   - Utilization of **Ridge Regression** to address multicollinearity and prevent overfitting.
   - Model training and validation using cross-validation with hyperparameter tuning.
   
4. **Deployment:**  
   - Serialization of the trained model using Pickle.
   - Integration of the model into a Flask web application that provides real-time predictions via an intuitive user interface.

## Technical Findings

- **Model Performance:**  
  The Ridge Regression model strikes a solid balance between bias and variance, resulting in reliable predictions even on unseen data.
  
- **Feature Importance:**  
  - **Location** and **Total Square Footage** emerged as the most influential predictors.
  - **BHK** and **Bathrooms** also contribute significantly, though to a slightly lesser extent.
  
- **Scalability:**  
  The predictive pipeline is optimized for real-time inference, making it suitable for integration into larger-scale applications.

## Business Insights

- **Market Trends Identification:**  
  Insights derived from the model highlight how different neighborhoods and property characteristics affect market prices.
  
- **Investment Decisions:**  
  Accurate price predictions aid investors and developers in assessing property values and mitigating risks.
  
- **Competitive Advantage:**  
  Integrating predictive analytics provides a strategic edge in pricing strategies and market positioning.
  
- **User Accessibility:**  
  The interactive web interface makes advanced analytics accessible to non-technical users.

## Hardware & Software Requirements and Libraries

- **Hardware Requirements:**
  - Modern CPU (dual-core or higher recommended)
  - Minimum 4GB RAM (8GB+ recommended for larger datasets)
  - Sufficient disk space for datasets and model files
  
- **Software Requirements:**
  - **Operating System:** Windows, macOS, or Linux
  - **Python Version:** 3.7 or higher
  - **Key Libraries:**
    - `pandas` & `numpy` for data manipulation and numerical analysis
    - `scikit-learn` for model building (Ridge Regression)
    - `Flask` for developing the web interface
    - `pickle` for model serialization
    - `Bootstrap` & `jQuery` for front-end development

## Getting Started

1. **Clone the Repository:**
   ```bash
   git clone <repository-url>
   cd HousePricePrediction


Screenshot of the project:

![image](https://user-images.githubusercontent.com/70855999/182067137-33171828-d922-4167-a5d5-22c0679a4ca2.png)
