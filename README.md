# Cadence , Speed Estimation and Foot strike 
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

## Speed Estimation
The next challenge was counting the number of cycles to estimate the speed of the treadmill, To calculate the speed we need the number of cycles multplied with the treadmill's deck length. 
For this Task I used YoloV3 and DeepSort to track the object and count the cycles number. The first step was training the model YoloV3 to detect the white tapes.The second step was to integrating the DeepSort algorithm with YoloV3 by transforming the model to Tensorflow model and tracking the whitetapes.The last step was counting the cycles using a virtual line ,and calculating the speed estimation with GT files.
