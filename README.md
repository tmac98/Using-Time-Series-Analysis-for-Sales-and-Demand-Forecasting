# 📚 Using Time Series Analysis for Sales and Demand Forecasting

## 📌 Project Overview  

This project explores time series forecasting techniques to predict weekly and monthly book sales for *The Alchemist* and *The Very Hungry Caterpillar*. The objective is to identify the most effective forecasting model for improving inventory planning and demand estimation. Various approaches—including traditional statistical models (SARIMA), machine learning (XGBoost), deep learning (LSTM), and hybrid models—were evaluated for their predictive accuracy.  

## 📊 Key Features  

- ✔️ **Data Preprocessing**: Cleaned and resampled weekly sales data, handling missing values and ensuring time-series continuity.  
- 📈 **Forecasting Models**: Evaluated SARIMA, XGBoost, LSTM, and hybrid models for sales prediction.  
- 📌 **Performance Metrics**: Used MAE (Mean Absolute Error) and MAPE (Mean Absolute Percentage Error) to assess forecasting accuracy.  
- 🛠 **Hyperparameter Tuning**: Optimised machine learning models for improved predictive performance.  
- 📊 **Comparative Analysis**: Assessed model effectiveness at both weekly and monthly forecasting levels.  

## 📈 Results & Insights  

- 🚀 **LSTM models** provided the most accurate forecasts at the weekly level.  
- 📌 **XGBoost** significantly outperformed SARIMA for monthly sales predictions.  
- 📊 **Hybrid models did not improve accuracy**, often introducing compounding residual errors.  
- 🤖 **SARIMA struggled** with capturing complex sales patterns, particularly for *The Very Hungry Caterpillar*.  
- 📉 **Stock replenishment strategies** should be based on LSTM for short-term forecasts and XGBoost for long-term planning.  

| Model | The Alchemist MAE | The Alchemist MAPE | The Very Hungry Caterpillar MAE | The Very Hungry Caterpillar MAPE |
|--------|-----------------|----------------|-----------------------------|-----------------------------|
| SARIMA | 155.08 | 0.2976 | 353.14 | 0.1863 |
| XGBoost | **94.99** | 0.1901 | 360.24 | 0.1687 |
| LSTM | **77.69** | **0.1524** | **314.93** | **0.1521** |
| Sequential Hybrid | 169.16 | 0.3719 | 476.75 | 0.2552 |
| Parallel Hybrid | 111.38 | 0.2027 | 482.81 | 0.2541 |
| Monthly XGBoost | 200.07 | **0.0791** | 703.80 | **0.0723** |
| Monthly SARIMA | 1326.63 | 0.4878 | 2863.04 | 0.3193 |

✔️ **Key Takeaway**:  
📌 **LSTM is the best choice for short-term forecasting**, while **XGBoost is optimal for long-term demand estimation**.  

## 📂 Project Files  

📄 **[Google Colab Notebook: Using Time Series Analysis for Sales and Demand Forecasting](./Using_Time_Series_Analysis_for_Sales_and_Demand_Forecasting.ipynb)**

📑 **[Business Report: Using Time Series Analysis for Sales and Demand Forecasting](./Using_Time_Series_Analysis_for_Sales_and_Demand_Forecasting.ipynb)**

## 🛠 Technologies Used  

- 🐍 **Python**: Pandas, NumPy, Scikit-Learn, TensorFlow, Matplotlib, Seaborn  
- 📈 **Time Series Modelling**: SARIMA, XGBoost, LSTM, Hybrid Models  
- 📊 **Visualisation**: Trend analysis, forecasting plots, error distributions  
- 🔍 **Optimization**: GridSearchCV, Keras Tuner, Auto ARIMA  

## 🔮 Future Improvements  

- 📊 **Explore external factors** (e.g., marketing campaigns, seasonal trends) to refine model accuracy.  
- 📈 **Develop an automated forecasting pipeline** to dynamically retrain models as new sales data becomes available.  
- 🖥️ **Deploy a real-time dashboard** for retailers and publishers to monitor predicted sales trends.  
