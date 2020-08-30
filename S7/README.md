# Session : 7

![GitHub top language](https://img.shields.io/github/languages/top/Shakil-1501/TSAI?label=Python)     ![Maintenance](https://img.shields.io/maintenance/yes/2020?logo=Github)          ![GitHub last commit](https://img.shields.io/github/last-commit/Shakil-1501/TSAI)   ![GitHub contributors](https://img.shields.io/github/contributors/SHAKIL-1501/TSAI) ![GitHub](https://img.shields.io/github/license/SHAKIL-1501/TSAI)

## Objective

  Train the CIFAR-10 Dataset and achieve accuracy of More than 80% on Conclusion Layer using below constraints.

   1. Architecture to C1C2C3C40 (basically 3 MPs) .
     
   2. Total Receptive Field must be more than 44.
     
   3. One of the layers must use Depthwise Separable Convolution.
     
   4. One of the layers must use Dilated Convolution.
     
   5. use GAP (compulsory):- add FC after GAP to target #of classes (optional) : ( ---- Not Used ---- )
     
   6. Achieve 80% accuracy, as many epochs as you want. Total Params to be less than 1M.
   
## Model Summary

```
----------------------------------------------------------------
        Layer (type)               Output Shape         Param #
================================================================
            Conv2d-1           [-1, 50, 32, 32]           1,400
              ReLU-2           [-1, 50, 32, 32]               0
       BatchNorm2d-3           [-1, 50, 32, 32]             100
            Conv2d-4          [-1, 100, 32, 32]          45,100
              ReLU-5          [-1, 100, 32, 32]               0
       BatchNorm2d-6          [-1, 100, 32, 32]             200
           Dropout-7          [-1, 100, 32, 32]               0
         MaxPool2d-8          [-1, 100, 16, 16]               0
            Conv2d-9          [-1, 200, 16, 16]           2,000
             ReLU-10          [-1, 200, 16, 16]               0
      BatchNorm2d-11          [-1, 200, 16, 16]             400
          Dropout-12          [-1, 200, 16, 16]               0
        MaxPool2d-13            [-1, 200, 8, 8]               0
           Conv2d-14          [-1, 500, 10, 10]         900,500
             ReLU-15          [-1, 500, 10, 10]               0
      BatchNorm2d-16          [-1, 500, 10, 10]           1,000
        MaxPool2d-17            [-1, 500, 5, 5]               0
           Conv2d-18             [-1, 10, 5, 5]          45,010
        AvgPool2d-19             [-1, 10, 1, 1]               0
================================================================
Total params: 995,710
Trainable params: 995,710
Non-trainable params: 0
----------------------------------------------------------------
Input size (MB): 0.01
Forward/backward pass size (MB): 7.39
Params size (MB): 3.80
Estimated Total Size (MB): 11.20

```
     
 ## Results    


- Acheived Accuracy = 78%
- Used Image Augmentation
- Number of Parameter : 995,710
- Number Of Epoch = 25
