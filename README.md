# Recurrent Neural Networks - Stock Price Prediction case study for MS - AI/ML
> This is a case study for Recurrent Neural Networks - Stock Price Prediction

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Predict the Stock Price for 4 IT Companies AMZN (Amazon), GOOGL (Google), IBM, MSFT (Microsoft)
- Load the data, data preparation, data aggregation, identify missing values
- Analyze and Visualize, data processing, decide predict window (in this case 30 days) and Split data
- Build RNN Model - Simple RNN, Tune Simple RNN, Advanced RNN using LSTM and GRU network 
- Perform hypertuning to find the optimal network configuration
- Predict Multiple target variables, Run the model and evaluate on the validation data set

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions

- The Stock Price Prediction of Recurrent Neural Networks (RNNs), specifically Simple RNNs, LSTMs, and GRUs, to predict stock prices for Amazon (AMZN), Google (GOOGL), IBM, and Microsoft (MSFT).

- Aimed to uncover patterns in historical stock data to forecast future price movements. Performed hyperparameter tuning to optimize model performance and evaluated the models using Root Mean Squared Error (RMSE) on the validation set.

### The Key Insights and Outcomes:
### Amazon (AMZN) Analysis
Observed very high RMSE values for the basic Simple RNN (1133993.07) and LSTM (1954368.96) models, indicating poor performance in predicting the 'Close' price with these architectures.

Multivariate Simple RNN for AMZN, predicting both 'Open' and 'Close' prices, yielded significantly lower RMSE values (13.67 for 'Open' and 15.03 for 'Close'). This suggests that modeling 'Open' and 'Close' prices together might be more effective than predicting 'Close' alone for AMZN within the tested architectures.

LSTM models for AMZN were tuned, with the best validation loss (0.0001) achieved with 70 units.

### Google (GOOGL) Analysis
For GOOGL, Simple RNN achieved its best performance with 30 units, resulting in a validation RMSE of 13.68.

LSTM performed best with 50 units, yielding a validation RMSE of 25.83.

GRU achieved the lowest validation RMSE for GOOGL (14.58) with 50 units, indicating a slight advantage of GRU over LSTM in this case.

### IBM Analysis
Simple RNN and GRU performed similarly well for IBM, achieving validation RMSE values of 2.44 (with 50 units) and 2.04 (with 30 units), respectively.

LSTM achieved a validation RMSE of 2.36 (with 30 units), slightly worse than Simple RNN and GRU.

IBM exhibited the lowest overall RMSE values across all stocks and model types, suggesting that its stock price might be more predictable based on the features used.

### Microsoft (MSFT) Analysis
Similar to IBM, MSFT also showed relatively lower RMSE values compared to AMZN and GOOGL.

GRU achieved the best performance for MSFT, with a validation RMSE of 1.43 (with 50 units).

Simple RNN (1.59 with 50 units) and LSTM (1.82 with 50 units) performed slightly worse than GRU.

#### Hyperparameter Tuning
The optimal number of units varied across stocks and model types, reinforcing the importance of hyperparameter tuning. For instance, the best Simple RNN for GOOGL had 30 units, while the best LSTM for GOOGL had 50 units.

### Model Comparison
#### GRU generally performed competitively, often achieving the lowest or comparable RMSE values across the different stocks, especially for GOOGL and MSFT. This suggests that GRUs might be a suitable choice for this type of stock price prediction task.

#### Simple RNN also demonstrated strong performance in some cases, particularly for IBM.

#### LSTM, while a powerful architecture, did not consistently outperform Simple RNN or GRU in this specific scenario.

## Conclusion
The study demonstrates that RNNs can capture temporal patterns in stock price data. However, the prediction accuracy varies significantly across different stocks.

- The models performed relatively well for IBM and MSFT, achieving lower RMSE values, while AMZN and GOOGL proved more challenging to predict.
- The choice of RNN architecture and hyperparameters plays a crucial role in model performance.
- GRUs showed promise in this analysis.
- These predictions are based solely on historical price data

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python Programming
- NumPy objects to create arrays/metrics to apply DL/ML modelsPython Programming
- Panda for Data Wrangling and Data manipulation purposes
- Seaborn to create visually appealing statistical graphics
- Matplotlib to create a range of plots and visualizations
- Iterator tool is to create iterator for efficient looping 
- Scikit Learn ML (Machine Learning) Library
- Keras is a high-level API for building and training NN (Neural Networks) on top of TensorFlow
- TensorFlow is an open-source ML framework for building and developing ML models
- All the versions are the latest as of April 2025

<!-- As the library versions keep on changing, it is recommended to mention the version of the library used in this project -->

## Acknowledgements
I want to credit upGrad for the Master of Science in Machine Learning and Artificial Intelligence (AI/ML) degree alongside IIIT-Bangalore, and LJMU, UK
- This project was inspired by all the Professors who trained us during the Recurrent Neural Networks, namely
  - G.Srinivasaraghavan - Professor, IIIT-B

## Contact
Created by [@rajaravisekara] - feel free to contact me, Raja - Sr Architect - AI Cloud


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
