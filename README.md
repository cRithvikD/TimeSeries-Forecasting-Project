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

As part of this analysis, we have fitted different models like SARIMAX, Theta, and Prophet.
Using Prophet gives us an RMSE of 183.3 on the training data, which we have used as part of our final submission!

## Acknowledgements:
1. Thanks to Dr. Shan Wang for organizing this competition as part of the 'MSDS 604: Time Series Analysis' course at USFCA!
2. Thanks to Aryan Mistry and Evan Turkon for being brilliant teammates!
