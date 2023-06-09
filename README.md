This repository presents a Time Series Forecasting project that focuses on analyzing over 10 years of hourly energy consumption data from PJM in Megawatts, sourced from the [Kaggle Dataset](https://www.kaggle.com/datasets/robikscube/hourly-energy-consumption). The objective of this project is to utilize XGBoost, a popular machine learning algorithm, for accurate forecasting.

<h2>Summary:</h2>


This repository comprises two parts. **[Part 1](part-1-time-series-forecasting-XGBoost.ipynb)** involves initial data analysis and visualization of various features, such as monthly energy consumption and hourly energy consumption. These visualizations provide insights into the dataset. Additionally, time series features are created based on the time series index. The dataset is then split into training and test sets, enabling the model to be trained using the XGBoost algorithm. To gain an understanding of the impact of each feature on the model, a feature importance analysis is conducted. Once the training is complete, the model is employed to forecast energy consumption on the test data. A plot is generated to showcase the true and predicted values, allowing for a visual comparison. Lastly, the root mean square error (RMSE) value is calculated to evaluate the accuracy of the forecasting model.

During the model training process, several hyperparameters are utilized. The "verbose" parameter is set to display training and validation scores at every 100 trees, providing insights into the model's performance. The "early_stopping_rounds" parameter is employed to prevent overfitting by stopping the training process before it reaches a point of diminishing returns. These measures ensure that the model is optimized and performs effectively for the task at hand.

**Real Data vs Predicted Data**
<img width="947" alt="Screenshot 2023-06-09 at 2 06 06 AM" src="https://github.com/tiashamondal29/Time-Series-Forecasting-using-XGBoost/assets/62413982/08b27a18-b8b4-49c5-b949-0d870acfff4c">

**[Part 2](part-2-time-series-forecasting-xgboost.ipynb)** of this repository delves into more advanced techniques in time series forecasting, including the following methods:

**Outlier Removal:** The dataset undergoes a rigorous outlier detection and removal process to ensure the accuracy and reliability of the forecasting models.

**Time Series Cross Validation:** A robust time series cross-validation strategy is employed to evaluate the performance of the forecasting models. This technique takes into account the temporal dependencies inherent in the data, allowing for a more realistic assessment of the models' predictive capabilities.

**Lag Features:** Lag features are generated to capture the temporal patterns and dependencies in the energy consumption data. These features enable the models to leverage past observations and their relationships with future values, enhancing the accuracy of the forecasts.

In the final section, the trained model is utilized to make future predictions for the upcoming year (2018-2019), providing valuable insights into the expected energy consumption patterns based on the historical data and the advanced forecasting techniques employed.

**Future Forecasting**

<img width="947" alt="Screenshot 2023-06-09 at 2 17 46 AM" src="https://github.com/tiashamondal29/Time-Series-Forecasting-using-XGBoost/assets/62413982/0320b11d-622b-46ce-9d4d-8de80e957c60">

