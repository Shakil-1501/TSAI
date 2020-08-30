# Sesssion : 8

## Objective : To Achieve 85% accuracy by training ResNet-18 Model on cifar10 dataset.

**Dataset** : CIFAR-10.

## Srategy 
Dataset is transformed with different Image Augmentation. Image Augmentation:

   - RandomHorizontalFlip(p=0.5)
   - RandomCrop(32, padding=2)
   - ColorJitter(brightness=0.1, contrast=0.1,saturation=0.1,hue=0.1) .

and Then Normalize.

 .

## Results:

Number Of Parameters : 11,173,962 ( Trainable parameters )

Accuracy : 88%

Epoch : 20



To Load and Run our Model . Kindly run the File : S8-Assignment.ipynb in google Colab and when asked upload the RestNetModel.py
