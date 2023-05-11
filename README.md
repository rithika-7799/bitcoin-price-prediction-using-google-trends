# Bitcoin price prediction using Google trends
### CS 651: Data-Intensive Distributed Computing final project

The project involved the development of a Bitcoin price prediction model 
using a combination of data from Bitcoin transaction blocks, 
historical prices, and Google Trends searches. To prepare the dataset for training, 
the Bitcoin transaction blocks were parsed from binary format to text and the required 
fields were extracted using a Python library, with a Spark implementation created for this purpose. 
Each data source was then worked on individually and indexed using a uniform timestamp format 
before being joined into a single dataframe for training and prediction.

The Linear Regression model was used to train the Bitcoin
data via the LinearRegression class of the PySpark ML library, 
with a pipeline built to prepare the data and fit the model. T
he model predicts the closing price for Bitcoin transactions, with its performance evaluated using RMSE and R-squared metrics.
