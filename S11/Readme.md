# Session : 11     

![GitHub top language](https://img.shields.io/github/languages/top/Shakil-1501/TSAI?label=Python)     ![Maintenance](https://img.shields.io/maintenance/yes/2020?logo=Github)          ![GitHub last commit](https://img.shields.io/github/last-commit/Shakil-1501/TSAI)   ![GitHub contributors](https://img.shields.io/github/contributors/SHAKIL-1501/TSAI) ![GitHub](https://img.shields.io/github/license/SHAKIL-1501/TSAI)

# Super Convergence

## Objective :

Write a code which uses this new ResNet Architecture for Cifar10:

---
- PrepLayer - Conv 3x3 s1, p1 >> BN >> RELU [64K ]

- Layer 1 
   * X = Conv 3x3 (s1, p1) >> MaxPool2D >> BN >> RELU [128k]
   * R1 = ResBlock( (Conv-BN-ReLU-Conv-BN-ReLU))(X) [128k] 
   * Add(X, R1)

- Layer 2 
   * Conv 3x3 [256k]
   * MaxPooling2D
   * BN
   * ReLU

- Layer 3 -
    * X = Conv 3x3 (s1, p1) >> MaxPool2D >> BN >> RELU [512k]
    * R2 = ResBlock( (Conv-BN-ReLU-Conv-BN-ReLU))(X) [512k]
    * Add(X, R2)

- MaxPooling with Kernel Size 4 and Stride 2
- Fully Connected Layer 
- SoftMax

---

*Use One Cycle Policy such that:*
- Total Epochs = 24
- Max at Epoch = 5
- LRMIN = FIND
- LRMAX = FIND
- NO Annihilation
 
 *Use this transform*
 - RandomCrop 32, 32 (after padding of 4) >> FlipLR >> Followed by CutOut(8, 8)
 - Batch size = 512
 - Target Accuracy: 90%.


## Results 
![LR Range Test Result Graph](https://github.com/Shakil-1501/TSAI/blob/master/S11/lrfinder.png)

- Maxium Learning Rate was found using LR-Range Test [Github Reference](https://github.com/davidtvs/pytorch-lr-finder/blob/master/torch_lr_finder/lr_finder.py)
  * Maximum LR = 0.01
- One Cycle Policy div_factor = 10
  * Initial Learning Rate = 0.01/10 = 0.001
- final_div_factor = 1 as NO Annihilation
 
 [Back To Top](#Super-Convergence)
 
 ## Files
 The IPYNB file can be found [here](https://github.com/Shakil-1501/TSAI/blob/master/S11/S11_Assignment.ipynb)
 
 Source code can be found below :
  * [CustomResNet Neural Network Model](https://github.com/Shakil-1501/TSAI/blob/master/S11/CustomResNet.py)
  * [Albumentation Transformation](https://github.com/Shakil-1501/TSAI/blob/master/S11/albumentationstransform.py)
  * [Data Loader](https://github.com/Shakil-1501/TSAI/blob/master/S11/dataloader.py)
  * [LR-Range Test](https://github.com/Shakil-1501/TSAI/blob/master/S11/LRScheduler.py)
  * [Training DataSet](https://github.com/Shakil-1501/TSAI/blob/master/S11/traindataset.py)
  * [Testing Dataset](https://github.com/Shakil-1501/TSAI/blob/master/S11/testdataset.py)
  
 - Best Validation Accuracy : 91%  
 

### Zig Zag Curve  One Cycle Policy Representation

   ![Zig-Zag Curve](https://github.com/Shakil-1501/TSAI/blob/master/S11/zigzag.png)
   
 ## Authors INFO
   
   Email : md.shakiluzzaman@gmail.com
   
   -[![](https://github.com/jagatabhay/TSAI/blob/master/logo.png)](https://www.linkedin.com/in/md-shakiluzzaman-894707129/)
[Back To Top](#Super-Convergence)
