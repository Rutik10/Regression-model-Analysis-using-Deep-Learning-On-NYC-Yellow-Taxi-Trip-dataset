# Regression-model-Analysis-using-Deep-Learning-On-NYC-Yellow-Taxi-Trip-dataset


Build a Deep Learning model (based on Neural Networks) that provides reliable and improved accuracy of
a NYC Yellow Taxi trip/ride duration.
You used the NYC/TLC Yellow Cab dataset, in Project #1, to find correlation among the various variables in
order to improve ride time predictions and predict the trip duration of a taxi ride taking into account the
different factors that affect the ride duration. Along with the above-mentioned dataset, one more file
should be included in your analysis, which involves the climatic conditions of the city.
Both of these datasets should be combined using pre-processing techniques to create a single dataset
that can be used further for accurate trip duration prediction.
Get the NYC climatic data from the Meteostat portal.
Here is the url to download the Jan-2020 climate data (*):
https://meteostat.net/en/place/3BBKPQ?t=2020-01-01/2020-01-31
(Note, the temperatures are in Celsius degrees and not in Fahrenheit!)


Perform regression modeling analysis on the ready-to-be-fed data into the following Neural Network
based algorithms:
1) MLP (Multi-Layer Perceptron)
2) Linear Regression (TF/Keras Sequential model w/ no hidden layers)
3) DNN (Deep Neural Network with at least 2 hidden layers)
Split your dataset into training and validation datasets in 80%/20% ratio.
(Note: Since dataset is time-sensitive, be extra careful on splitting…)
At the compiling phase, use:
 loss function: Mean Square Error (MSE), Mean Absolute Error (MAE).
 optimizer: SGD, Adam, RMSProp.
o Use various values for learning rate (lr)
After each fit (run each one for a single value of epoch=100), present/plot the training_loss vs
validation_loss (could utilize TensorBoard GUI module)
Present the best Regression Deep Learning model (compare the above 3) and its corresponding
parameters. Assume bacth_size takes its default value of 32.
Using the best selected regression model, perform predictions by calling Keras model.predict module and
review the loss.
Be aware of the following:
A) Mean square error (MSE) and mean absolute error (MAE) are common loss functions used for
regression problems. MAE is less sensitive to outliers.
B) When numeric input data features have values with different ranges, each feature should be scaled
independently to the same range.
C) Overfitting is a common problem for DNN models
(*) While at the Meteostat portal, select ‘location’ (New York, Wall Street) and ‘date range’ (01/01/2020
to 01/31/2020).
