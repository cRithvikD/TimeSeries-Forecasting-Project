# TimeSeries-Forecasting-Project

## Data:
Renewable energy remains one of the most important topics for a sustainable future.
Wind, being a perennial source of power, could be utilized to satisfy our power
requirements. With the rise of wind farms, wind power forecasting would prove to be
quite helpful.
Here's data on a particular windmill. It contains various weather, turbine, and rotor
features. Data has been recorded from January 2018 till March 2020. Readings have
been recorded at 10-minute intervals. The aim was to predict the mean daily wind
power that could be generated from the windmill for the next 15 days.

## Goal of this project:
Use the training data (‘train.csv’) to select and train a model to produce a forecast on
the mean daily wind power that could be generated from the windmill for the next 15
days. The target variable indicating the wind power is the column ‘ActivePower’ in the
training set. The prediction accuracy will be measured using RMSE.

## The analysis: 

As part of this analysis, we have fitted different models like SARIMAX, Theta, and Prophet.

1. First off, we started by estimating the p,d,q,P,D,Q,m values from the ACF and PACF plots, and used the ADF test to understand if it is stationary. After fitting the SARIMAX model, we get the best model as SARIMAX((0, 0, 1)), ((6, 0, 3, 21)) with an RMSE: 290.7818112299762
   
2. Next, we fit a theta model with a period of 31 days, however the RMSE wa 240.1, not much of an improvement
   
3. Finally, fitting a Prophet model with a period=21 and fourier order=1 gave us an RMSE of 183.3 on the training data, and this is what we have used as part of our final submission!

## Acknowledgements:
1. Thanks to Dr. Shan Wang for organizing this competition as part of the 'MSDS 604: Time Series Analysis' course at USFCA!
2. Thanks to Aryan Mistry and Evan Turkon for being brilliant teammates!
