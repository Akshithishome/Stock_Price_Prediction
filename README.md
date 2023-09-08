# Stock_Price_Prediction using Stacked LSTM

**Problem Statement:** 
The stock market is a complex system that is influenced by a variety of factors, including economic conditions, political events, and investor sentiment. It is difficult to predict the future price of a stock with certainty. The objective of this project is to develop a machine-learning model that can predict the future price of a stock with a high degree of accuracy. This model can be used by investors to make more informed investment decisions.
The main metric used to measure the accuracy is **RMSE(Root Mean Squared Error)**.

Technologies used:
1. pandas
2. pandas datareader
3. numpy
4. matplotlib
5. TensorFlow
6. keras

**Approach:**
1. Data Collection - Used pandas_datareader to access open-source websites to get access to the API key and save it into a CSV file.
2. Pre-processing - Mainly the closing value of the stock is taken for each date, and used MinMaxScaler to normalize the data between (0,1).
3. Model Training - Used Stacked **LSTM with Adam Optimizer** after splitting the data as such, 65% for training and 35% for testing.
4. Prediction - After calculating the RMSE values for train data and test data which are "**216.28223294235866**" and "**152.42438442804368**" respectively, there isn't much difference showing our model is good and the outputs are plotted

![image](https://github.com/Akshithishome/Stock_Price_Prediction/assets/105364531/f4659356-6e33-4b70-81eb-7e4711c46e6e)

6. Forecasting for after 30 days by using the previous 100 observations in the data

![image](https://github.com/Akshithishome/Stock_Price_Prediction/assets/105364531/e31db410-675a-4bf7-b810-f1ffafbbf679)

6. After combining

![image](https://github.com/Akshithishome/Stock_Price_Prediction/assets/105364531/21a85d14-c007-4296-84b6-0c26d20317f6)

7. Overall Forecast plot

![image](https://github.com/Akshithishome/Stock_Price_Prediction/assets/105364531/75e570b6-1ecd-4b00-9a25-ddc4ff290d67)


**Future Improvements:**
Taking into consideration of Covid the above model was designed as assumed to be not abnormal, I would like to forecast the same 10 days after excluding the stocks prior Covid pandemic and check the error see whether if it does affect the prediction or not.





