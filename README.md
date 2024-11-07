# 📈 Sales Forecasting using Time Series Analysis

Welcome to the **Sales Forecasting Project**! This project leverages time series models to forecast monthly sales for inventory planning and marketing strategy optimization. Using the [Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/online+retail) from the UCI Machine Learning Repository, this analysis covers data preprocessing, model selection, and forecasting using ARIMA and SARIMA models. 

## 🗂 Project Structure
├── data/ # Contains the raw data (e.g., Online Retail.xlsx)
├── notebooks/ # Jupyter notebooks for exploratory data analysis and modeling 
├── src/ # Source code for model building and evaluation 
├── results/ # Forecasted sales and visualizations 
└── README.md # Project README


## ✨ Key Features
- **Exploratory Data Analysis** to understand sales patterns and seasonality
- **Data Preprocessing** for handling missing values, outliers, and formatting data
- **Model Building** with ARIMA and SARIMA for time series forecasting
- **Forecast Visualization** for easy interpretation of results
- **Error Analysis** to ensure model reliability and stability

## 🚀 Project Goals
1. **Accurate Sales Forecasts**: Support inventory planning and marketing strategies with accurate forecasts.
2. **Understanding Sales Patterns**: Analyze seasonal and trend components in the sales data.
3. **Deployable Solution**: Provide an adaptable forecasting framework for similar sales data.

## 📊 Data Overview
The dataset contains sales data from an online retail company, with information on:
- **Invoice Number** - Unique number for each transaction
- **StockCode** - Product/item code
- **Description** - Product description
- **Quantity** - Quantity of products purchased
- **InvoiceDate** - Date of transaction
- **UnitPrice** - Price per unit
- **CustomerID** - Unique identifier for each customer
- **Country** - Country of purchase

**Note**: The data includes missing values and requires preprocessing.

## ⚙️ Methodology

1. **Exploratory Data Analysis (EDA)**: Visualized seasonal trends, monthly sales, and outlier patterns.
2. **Data Transformation**: Addressed missing values, formatted data to monthly aggregation, and logged transformations to stabilize variance.
3. **Stationarity Tests**: Used ADF and KPSS tests to check stationarity.
4. **Model Selection**: Based on ACF/PACF, we chose the best-fit ARIMA and SARIMA models.
5. **Model Evaluation**: Conducted residual analysis and the Ljung-Box test to confirm model adequacy.
6. **Forecasting**: Forecasted monthly sales with confidence intervals.

## 📉 Model Performance
### ARIMA Model Summary:
After testing different (p, d, q) values, the ARIMA model achieved satisfactory results with the following configuration:
- **Order**: ARIMA(1, 1, 1)
- **Performance**: The model captures trends effectively, with forecasted sales values aligning well with expected patterns.

### SARIMA Model Summary:
The SARIMA model was applied to capture seasonality, achieving stable results and overcoming residual autocorrelation. 

## 🔍 Results & Insights

### Forecasted Sales Values:
| Date       | Forecasted Sales |
|------------|------------------|
| 2012-01-31 | 1,047,047        |
| 2012-02-29 | 860,605          |
| 2012-03-31 | 917,276          |
| ...        | ...              |

### Confidence Intervals for Forecasted Sales:
| Date       | Lower Sales   | Upper Sales   |
|------------|---------------|---------------|
| 2012-01-31 | 401,027       | 1,693,067     |
| 2012-02-29 | 196,317       | 1,524,893     |
| 2012-03-31 | 186,711       | 1,647,841     |
| ...        | ...           | ...           |


## 📈 Visualization Examples
![Forecasted Sales Plot](./results/forecast_plot.png)
*Example of visualizing monthly sales forecasts with confidence intervals.*
![image](https://github.com/user-attachments/assets/f78d7505-b44f-40a7-a846-26dc54666b99)



## 🚀 How to Use This Project

1. **Clone this repository**:
   ```bash
   git clone https://github.com/PranayaKD/sales-forecasting.git
   cd sales-forecasting

## 🛠 Future Enhancements
- **Automated Hyperparameter Tuning**: Implement grid search for ARIMA/SARIMA parameters.
- **Seasonality Detection**: Add automated seasonality detection for other potential patterns.
- **Model Comparison**: Test advanced models like Prophet or LSTM for comparison.

## 📜 License
This project is licensed under the MIT License. See the `LICENSE` file for more details.

## 🙋‍♂️ Contact
Feel free to reach out for collaboration or questions! Connect with me on [LinkedIn](https://linkedin.com/in/pranayakd28) or view more projects on [GitHub](https://github.com/PranayaKD).

---

### ⭐️ Acknowledgements
Thanks to the UCI Machine Learning Repository for the dataset and the open-source community for inspiration.

---

Thank you for visiting! 😊 Happy forecasting!




