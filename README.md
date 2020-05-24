# Long-short-term-memory-LSTM-on-Time-Series-Airline-Passengers-Dataset-Data
This is a very short exploration into applying LSTM techniques using the Keras library. Code and content is based on several cool blog posts and papers; see references section for more info.

# Airline Passenger Data
In this example we wish to make forcasts on a time series of international airline passengers.

The time series data forcast can be modeled as a univariate regression-type problem, concretely let  𝑋𝑡  denote the number of airline passengers in month  𝑡 . Then: 𝑋𝑡=𝑓(𝑋𝑡−1,Θ), 

which I aim to solve using the a simple LSTM neural network.

Here  𝑋𝑡  is the number of passengers at time step  𝑡 ,  𝑋𝑡−1  denotes number of passengers at the previous time step, and  Θ  refers to all the other model parameters, including LSTM hyperparameters.

Note: For better readability, in the code for this as well as the next example, the predicted new value at time step  𝑡  is written as Y.

## Results
Predictions and model evaluation: As seen in model notebook, already the simple model performs not too poorly. The advantage of using the RMSE is that it's in the same unit as the original data, i.e. 1.000 passengers / month.

Training data score: 21.46 RMSE
Test data score: 53.37 RMSE
