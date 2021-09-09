# Cadence and Foot strike 
## This code can be used to count excerises, like push ups etc..
In this repo you will find the Cadence counter algorithms to estimate the number of steps per minute.
We used two algorithms to count the number of steps.

## The Pose Estimation + KNN 
In this algorithm we trained the KNN model with small dataset (100 samples of left and right steps)
We got good result compared to GT results.

![Pose Estimation with KNN](https://github.com/aimanyounises1/Cadence_Counter/blob/c19d13dac8ba826bf3c97c2d551c385036022dcb/Pose%20Estimtion%20with%20KNN.png)

## The RepNet Trial
With RepNet we got 35 cycles which it's almost 70 steps, the GT steps were 76 steps.
![RepNe](https://github.com/aimanyounises1/Cadence_Counter/blob/c19d13dac8ba826bf3c97c2d551c385036022dcb/RepNet.png)
