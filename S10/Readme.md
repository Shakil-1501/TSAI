# Session : 10

![GitHub top language](https://img.shields.io/github/languages/top/Shakil-1501/TSAI?label=Python)     ![Maintenance](https://img.shields.io/maintenance/yes/2020?logo=Github)          ![GitHub last commit](https://img.shields.io/github/last-commit/Shakil-1501/TSAI)   ![GitHub contributors](https://img.shields.io/github/contributors/SHAKIL-1501/TSAI) ![GitHub](https://img.shields.io/github/license/SHAKIL-1501/TSAI)

## Objective

- Pick your last code
- Make sure  to Add CutOut to your code. It should come from your transformations (albumentations)
- Use this repo: https://github.com/davidtvs/pytorch-lr-finder (Links to an external site.) 

  - Move LR Finder code to your modules
  - Implement LR Finder (for SGD, not for ADAM)
  - Implement ReduceLROnPlatea: https://pytorch.org/docs/stable/optim.html#torch.optim.lr_scheduler.ReduceLROnPlateau (Links to an external site.)
  
- Find best LR to train your model
- Use SDG with Momentum
- Train for 50 Epochs. 
- Show Training and Test Accuracy curves
- Target 88% Accuracy.
- Run GradCAM on the any 25 misclassified images. Make sure you mention what is the prediction and what was the ground truth label.

## Approach

**Albumentations code**

```python
import torch
import torchvision
import torchvision.transforms as transforms
import torch.nn as nn
import torch.nn.functional as F

mean = (0.4914, 0.4822, 0.4465)
std = (0.2023, 0.1994, 0.2010)

trans = transforms.Compose([ transforms.ToTensor(),
                             transforms.Normalize(mean, std)
                            ])

from albumentations import Compose, RandomCrop, Normalize, HorizontalFlip, VerticalFlip, Resize,Rotate , Cutout
from albumentations.pytorch import ToTensor
import numpy as np

class train_transforms():

    def __init__(self):
        self.albTrainTransforms = Compose([  # Resize(256, 256),
            Rotate((-10.0, 10.0)),
            HorizontalFlip(p=0.5),
            VerticalFlip(p=0.5),
            Cutout(num_holes = 8, max_h_size = 8, max_w_size = 8),
            Normalize(mean=[0.5, 0.5, 0.5], std=[0.5, 0.5, 0.5]),
            ToTensor()
        ])# this is train transforms

    print("REQUIRED LIBRARIES LOADED...")

    def __call__(self, img):
        img = np.array(img)
        img = self.albTrainTransforms(image=img)['image']
        return img
        
  ```
  ## Logfile for training
  
  ```
  
[1,   900] loss: 1.775
[2,   900] loss: 1.356
[3,   900] loss: 1.150
[4,   900] loss: 1.037
[5,   900] loss: 0.927
[6,   900] loss: 0.856
[7,   900] loss: 0.803
[8,   900] loss: 0.749
[9,   900] loss: 0.723
[10,   900] loss: 0.694
[11,   900] loss: 0.649
[12,   900] loss: 0.630
[13,   900] loss: 0.611
[14,   900] loss: 0.580
[15,   900] loss: 0.545
[16,   900] loss: 0.546
[17,   900] loss: 0.524
[18,   900] loss: 0.510
[19,   900] loss: 0.504
[20,   900] loss: 0.484
[21,   900] loss: 0.468
[22,   900] loss: 0.456
[23,   900] loss: 0.460
[24,   900] loss: 0.437
[25,   900] loss: 0.431
[26,   900] loss: 0.414
[27,   900] loss: 0.408
[28,   900] loss: 0.391
[29,   900] loss: 0.384
[30,   900] loss: 0.390
[31,   900] loss: 0.378
[32,   900] loss: 0.367
[33,   900] loss: 0.362
[34,   900] loss: 0.356
[35,   900] loss: 0.345
[36,   900] loss: 0.344
[37,   900] loss: 0.329
[38,   900] loss: 0.329
[39,   900] loss: 0.327
[40,   900] loss: 0.319
[41,   900] loss: 0.312
[42,   900] loss: 0.306
[43,   900] loss: 0.309
[44,   900] loss: 0.307
[45,   900] loss: 0.300
[46,   900] loss: 0.296
[47,   900] loss: 0.287
[48,   900] loss: 0.283
[49,   900] loss: 0.287
[50,   900] loss: 0.281
Finished Training

```
## Results

- Accuracy of the network on the 10000 test images: 85 %
 
