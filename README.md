# Power_forecast_Tensorflow
In this project I used stacked LSTM from Tensorflow to forecast future power consumption. Some summaries of the project:

1) Global Power In(GPI) can be forecasted as a stand-alone time series since it does not depend on VPS system. It might depend on utility service (PG&E,..)

2) Global Power Out(GPO) is too bumpy to have a good forecast to track all the spikes, so forecast lines are very close to a smooth average.

3) Difference between GPI and GPO can have a good forecast. It also benefits from adding other variables e.g voltage, intensity, room metters.

4) There is potential to improve on forecast error with increase number of epochs and finetune model architecture. Most of loss curve are not flat yet.
