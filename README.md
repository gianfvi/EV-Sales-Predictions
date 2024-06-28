# Predictive Analysis of EV/PHEV Sales for Dealerships

## Project Overview

This project aims to analyze historical sales data of Electric Vehicles (EVs) and Plug-in Hybrid Electric Vehicles (PHEVs) to predict future sales trends. The analysis provides insights into growth patterns, market dynamics, and infrastructure needs, aiding a dealership in strategic planning and investment decisions.

## Data Sources

The study utilizes data from the following sources:
- US Department of Energy
- Local DMVs of California, Florida, New York, Texas, and Washington
- U.S. Census Bureau
- U.S. Energy Information Administration
- Bureau of Labor Statistics
- The World Data Bank

## Data Cleaning and Wrangling

Cleaning and wrangling the data involved:
- Focusing on a 10-year period for state-specific data
- Using recent data for U.S. general data
- Ensuring data was cleaned and processed for predictive analysis

## Notebooks

1. **Machine Learning Predictive Analysis.ipynb**
2. **States Notebook.ipynb**

## Machine Learning Predictive Analysis

### Contents

1. **Data Loading and Preparation**
   - Loading the dataset
   - Converting 'Date' column to datetime format
   - Setting the date column as the index
   - Cleaning 'Gas Vehicles sales' column

2. **Data Visualization**
   - Visualizing trends for Hybrid/EV sales, gas vehicle sales, gas prices, diesel prices, unemployment rate, and inflation rate

3. **Correlation Analysis**
   - Calculating and displaying the correlation matrix

4. **Feature Engineering and Normalization**
   - Adding polynomial features
   - Normalizing the data

5. **Model Training and Tuning**
   - Defining models (Random Forest, Gradient Boosting)
   - Hyperparameter tuning using GridSearchCV

6. **Ensemble Modeling**
   - Creating and evaluating an ensemble model combining the best-tuned models

7. **Feature Importance and Predictions**
   - Visualizing model predictions vs. actual values
   - Plotting feature importances for both Random Forest and Gradient Boosting models

## States Notebook

### Contents

1. **Data Loading**
   - Importing state-specific data from various sources

2. **Data Cleaning and Processing**
   - Cleaning and wrangling state-specific data for analysis

3. **Exploratory Data Analysis (EDA)**
   - Visualizing state-specific trends and patterns

4. **Model Development**
   - Developing and tuning models for state-specific predictive analysis

5. **Model Evaluation**
   - Evaluating model performance using appropriate metrics

## Conclusion

The predictive analysis indicates a strong growth trajectory for EV/PHEV sales, with estimates between 200,000 and 500,000 units. For the dealership, this suggests a significant opportunity to expand EV/PHEV inventory and enhance charging infrastructure. By leveraging these predictions, the dealership can capitalize on market trends, ensuring long-term growth and leadership in the EV market.

## Repository Structure

```plaintext
.
├── Machine Learning Predictive Analysis.ipynb
├── States Notebook.ipynb
├── README.md
└── data
    ├── ML_DATASET.csv
    ├── CA_data.csv
    ├── FL_data.csv
    ├── NY_data.csv
    ├── TX_data.csv
    ├── WA_data.csv
```

## How to Run the Project

1. Clone the repository.
2. Ensure all data files are in the `data` directory.
3. Open and run the notebooks in Jupyter Notebook or JupyterLab.
4. Follow the steps in each notebook to reproduce the analysis and predictions.

## Dependencies

- pandas
- matplotlib
- seaborn
- scikit-learn
- xgboost
- catboost
- statsmodels

Install the dependencies using pip:

```bash
pip install pandas matplotlib seaborn scikit-learn xgboost catboost statsmodels
```

## Author

Gian F. Villafañe Morales - Data Analyst

## License

This project is licensed under the MIT License.
