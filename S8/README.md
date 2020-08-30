# Sesssion : 8

![GitHub top language](https://img.shields.io/github/languages/top/Shakil-1501/TSAI?label=Python)     ![Maintenance](https://img.shields.io/maintenance/yes/2020?logo=Github)          ![GitHub last commit](https://img.shields.io/github/last-commit/Shakil-1501/TSAI)   ![GitHub contributors](https://img.shields.io/github/contributors/SHAKIL-1501/TSAI) ![GitHub](https://img.shields.io/github/license/SHAKIL-1501/TSAI)

## Objective 

 To Achieve 85% accuracy by training ResNet-18 Model on cifar10 dataset.

**Dataset** : CIFAR-10.

## Strategy 

Dataset is transformed with different Image Augmentation. Image Augmentation:

   - RandomHorizontalFlip(p=0.5)
   - RandomCrop(32, padding=2)
   - ColorJitter(brightness=0.1, contrast=0.1,saturation=0.1,hue=0.1) .

and Then Normalize.

## Model training summary

```
[1,   900] loss: 1.594
[2,   900] loss: 0.974
[3,   900] loss: 0.737
[4,   900] loss: 0.615
[5,   900] loss: 0.553
[6,   900] loss: 0.482
[7,   900] loss: 0.440
[8,   900] loss: 0.404
[9,   900] loss: 0.366
[10,   900] loss: 0.341
[11,   900] loss: 0.318
[12,   900] loss: 0.297
[13,   900] loss: 0.279
[14,   900] loss: 0.260
[15,   900] loss: 0.239
[16,   900] loss: 0.227
[17,   900] loss: 0.220
[18,   900] loss: 0.205
[19,   900] loss: 0.203
[20,   900] loss: 0.181
Finished Training

```



## Results:

- Number Of Parameters : 11,173,962 ( Trainable parameters )

- Accuracy : 88%

- Epoch : 20



To Load and Run our Model . Kindly run the File : [link](https://github.com/Shakil-1501/TSAI/blob/master/S7/S7_Assignment.ipynb) in google Colab and when asked upload the RestNetModel.py

## Authors INFO
   
   Email : md.shakiluzzaman@gmail.com
   
   -[![](https://github.com/jagatabhay/TSAI/blob/master/logo.png)](https://www.linkedin.com/in/md-shakiluzzaman-894707129/)
