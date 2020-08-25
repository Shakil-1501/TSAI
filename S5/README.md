# Session: 5


## Objective




 In this project we will train the model with MNIST dataset and to achieve 
  99.40% accuracy (not once but for consistently  4 epoch ) within 5-15 epoch without
  using fully connected layer.
 And to achieve this we have a constraint of not using more than 10K parameters.

Our Model is Based on Convolution Neural Network ( CNN ) .

So we had divided the problems into multiple parts and then tried to 
 train the model by correcting features step by step sequentially
 till the target accuracy is achieved like listed below:
 
1. Building Lighter Model.
    
2. Batch Normalization.

3. Use Dropout in proper place.

4. Global Average Pooling.

5. Image Augmentation techniques.

6. Learning Rate(LR) Scheduler.

## Result :

  We had successfully achieve the target accuracy of 99.40% .
  1. Parameters            : 9736
  2. Best Train Accuracy   : 98.09%
  3. Best Test Accuracy    : 99.45%

## Observation

- we have maintained  the model to not "OVERFIT".
- We have achieved better accuracy by doing slightly image rotation 
  and step size of LR to reduce after 5 step.

 ( We obtained this by hit and trail and upon rigorous analysing ).


  Well "Excess of Anything is not Bad. It is Worst ....!! ".
  Same thing happens to us.
  But it is worth for someone, who is in a learning phase.

  But tried multiple ways to achieve the target.

## Points to Remember

 1. Choose the batch size wisely.
 
 2. To achieve high accuracy , first epoch should give good accuracy.
 
 3. Never apply Relu , Dropout , Batch Normalization at the last convolution Layer.


                      ------------------Thanking You-------------------------
