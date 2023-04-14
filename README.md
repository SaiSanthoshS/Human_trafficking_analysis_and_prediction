# Human_trafficking_analysis_and_prediction
##Arima model:

A dataset on human trafficking for the years 2015-2020 has been loaded and trains a SARIMA model on the data for each state in India. It then makes predictions for the next 5 years using each trained model and plots the actual and predicted values for each state.

The code first imports the required libraries: Pandas, NumPy, Statsmodels, and Matplotlib. It then loads the dataset using Pandas and extracts the list of states from the first column. It creates two empty dictionaries, "models" and "predictions", to store the trained models and predicted values for each state.

The code then loops over each state and trains a separate SARIMA model using the Statsmodels library. It splits the data into training and testing sets, trains the model using the training data, and makes predictions for the next 5 years using the "forecast" method. It stores the trained model and predicted values in the "models" and "predictions" dictionaries.

Finally, the code loops over each state again and creates a plot of the actual and predicted values for each state using Matplotlib. It retrieves the actual values from the dataset, concatenates them with the predicted values, and plots them on a line graph with the year on the x-axis and the number of cases on the y-axis. The plot is then displayed using the "show" method