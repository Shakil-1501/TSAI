# Session : 12

## Objective

### Assignment A:

- Download this TINY IMAGENET (Links to an external site.) dataset. 
- Train ResNet18 on this dataset (70/30 split) for 50 Epochs. Target 50%+ Validation Accuracy. 
- Submit Results. Of course, you are using your own package for everything. You can look at this (Links to an external site.) for reference. 

### Assignment B:
- Download 50 images of dogs. 
- Use this (Links to an external site.) to annotate bounding boxes around the dogs.
- Download JSON file. 
- Describe the contents of this JSON file in FULL details (you don't need to describe all 10 instances, anyone would work). 
- Refer to this tutorial (Links to an external site.). Find out the best total numbers of clusters. Upload link to your Colab File uploaded to GitHub. 


### Approach for Assignment A

- The code is made modular by keeping traindatest,testdataset and dataset loader as seperate file
- Downloading TINY IMAGENET dataset 
- Using SGD optimizer and cross EntropyLoss  as loss function
- Using LR Finder as scheduler
- Train Resnet18 on this dataset for 20 epochs.

### Results:

- Accuracy of the Network on the 10000 test images: 53 %

### Approach for Assignment B

statistics graph

![1](https://user-images.githubusercontent.com/63920152/92770027-2c899400-f3b7-11ea-8f86-d80e3f841134.png)

![2](https://user-images.githubusercontent.com/63920152/92770037-2eebee00-f3b7-11ea-9dcd-ad182947915f.png)

