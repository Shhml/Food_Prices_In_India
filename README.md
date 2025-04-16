# Food_Prices_In_India
## 🥘 Food Prices in India – EDA & Price Prediction 

This project performs Exploratory Data Analysis (EDA) and builds a Linear Regression model to predict food prices across different states and markets in India. The analysis is done using Google Colab with a clean workflow covering data preprocessing, visualization, and prediction.

## 📌 Project Workflow (Step-by-Step)

## Step 1: Data Loading and Initial Exploration

- Imported the dataset using Pandas.
- Displayed the first few rows using .head() to understand the structure.
- Checked dataset info with .info() and .describe() to inspect:
- Data types
- Null/missing values
- Basic statistics

## Step 2: Data Cleaning

- Converted the date column to datetime format.
- Handled missing and zero values:
- Removed rows with 0 or null in modal price, min, or max price columns.
- Ensured the dataset is clean for further analysis and modeling.

## Step 3: Exploratory Data Analysis (EDA)
📊 Key Analyses Performed:
- Counted unique values of:
- Commodities
- State
- Centers (Markets)
- Found the most frequently recorded commodities.
- Visualized price trends over time for selected commodities.

## 📈 Visualizations Included:

- Line plots showing how modal prices change over time.
- Boxplots comparing price distributions between states and commodities.
- Bar charts for top and bottom states by average price.

## Step 4: Feature Engineering

## Extracted new features from the date column:
- Year
- Month
## Converted categorical columns into numeric format using Label Encoding:
- State
- Center
- Commodity

## Step 5: Building the Price Prediction Model
## 🧠 Model Details:

- Selected Modal Price as the target variable.
- Selected input features:
- Encoded State, Center, Commodity
- Year, Month from date
- Split data into train and test sets using train_test_split.
- Trained a Linear Regression model using Scikit-learn.

## ✅ Model Evaluation:

- Evaluated performance using:
- R² Score
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Plotted Predicted vs. Actual Prices to visualize model accuracy.

## Step 6: Insights & Observations

- Metro cities tend to have higher modal prices than smaller towns.
- Some commodities show seasonal pricing trends.
- Data cleaning significantly improved model performance.
- Linear Regression captures basic patterns, but more complex models could improve prediction.

## 🚀 Tools & Libraries Used Google Colab

- Pandas, NumPy – data wrangling
- Matplotlib, Seaborn – visualization
- Scikit-learn – machine learning and model evaluation

## 🔮 Future Improvements

- Try Random Forest or XGBoost for better predictions.
- Build a time-series model like ARIMA or Prophet for forecasting.
- Add external data like rainfall, inflation, or crop data.
- Develop an interactive dashboard using Streamlit or Dash.
