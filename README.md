# Applied Deep Learning : Convolution Neural Network

![PyPI - Python Version](https://img.shields.io/pypi/pyversions/3)
![Maintenance](https://img.shields.io/maintenance/yes/2020)
![GitHub last commit](https://img.shields.io/github/last-commit/Shakil-1501/TSAI)
![GitHub contributors](https://img.shields.io/github/contributors/Shakil-1501/TSAI)


## REPO Discription

   This repository is all about Computer Vision on Pytorch Framework

## Prerequisite

- Python
- Pytorch and basics of Opencv

<details>
<summary>ML Intituation and basics of CNN</summary>

[Work-Link]()

This describes the very basics of Python, i would recommend binge watching Raymond Hettinger's YouTube Videos, as much as you can, also learn list comprehension, slicing, partial, functools, functional programming, classes, MRO, decorators, lambdas, python 3 typing

Also here i learnt the basics of how a Neural Network learns, how the different channels are formed, what are kernels, how does the DNN make sense of the input it gets, and more !

Have you ever wondered, like why do we only use 3x3 kernels ? i had always wondered, why not 5x5 ? 7x7 ? in this session i learnt why, and how does even the kernel size matter ? why is it only odd numbers ? and why only squares ? and why is 3x3 kernel used twice same as a 5x5 kernel, what is receptive field ?

</details>

<details>
<summary>Neural Architecture</summary>

[Work-Link]()

This describes the basic neural network architecure, see its page for details

</details>

<details>
<summary>Kernels,Convolutions and Activation Function</summary>

[Work-Link]()

Basic Pytorch architecture for working with neural networks, introduces you to nn.Module, optimizers, forward and backward pass, datasets, how to apply simple augmentation.

</details>

<details>
<summary>Architecture Basics</summary>

[Work-Link]()

Here we had to train MNIST to get 99.4% accuracy with some given contraints, was quite fun to do this, got me out of the noob shell of what a neural network actually is and what it does, because i had to write code manually, not copy paste any more.

</details>

<details>
<summary>Model Implementation</summary>

[Work-Link]()

This was very important to realise the basic steps required to make a neural network and then go on to optimize it, to get the perfect model size and accuracy, very important, please see its documentation, and all the notebooks

</details>

<details>
<summary>Batch Normalization and Regularization</summary>

[Work-Link]()

This  focuses on the importance of normalization and regularization in neural networks, aim was to also get > 99.4% accuracy in less than 40 epochs for MNIST with limited model parameters

</details>

<details>
<summary>Advanced Convolutions</summary>

[Work-Link]()

Here i was introduced to various convolution types you can add in the network, we were given a custom network which we had to implement, also we had to make a custom library of python to support and ease the process of NN building and training,

</details>

<details>
<summary>Receptive Fields and different Network Architecture</summary>

[Work-Link]()

Here i was introduced to ResNet18 and CIFAR dataset with aim to get 85% test accuracy



</details>

<details>
<summary>Data Augmentation</summary>

[Work-Link]()

This was amazing, i was introduced to GradCAM, and i myself learnt about saliency map



</details>

<details>
<summary>Training and Learning Rates</summary>

[Work-Link]()

Here i had to use LR Finder to find the best learning rate for the model, i also used OneCyclePolicy for faster convergence. i reached 92.03% accuracy in CIFAR using ResNet18

</details>

<details>
<summary>Super-Convergence</summary>

[Work-Link]()

A custom architecture was implemented here, along with that i used OneCycleLR to improve the convergence of the NN

</details>

<details>
<summary>Object Localization</summary>

[Work-Link]()

Here we had to do image annotation and collect doggo dataset.

Also i had to make a custom dataloader and dataset class in PyTorch to support TinyImageNet, and then train a model to reach 60% accuracy, which i failed to, but still i learnt from my mistakes ! the one who doesnt make mistakes does really make anything does he ?

</details>

<details>
<summary>YOLO-2 & 3</summary>

[Work-Link]()

I was introduced to YOLO, something i always wondered how it exactly worked, and why is it called YOLO ? now i understand why. and people complain about the FPS of YOLO, now i know why, they dont pay attention to the anchor boxes, which is very important and its different for different datasets.

I made a custom Bugs Bunny detector using the YOLO architecture :) i like my detector :) i like bugs bunny :) i custom collected bugs bunny images, self annotated about 600 images of my bunny and trained the network for like 5 hours on a Tesla P100

</details>

<details>
<summary>RCNN</summary>

[Work-Link]()

I was introduced to RCNN family and SSD, but that wasnt the main thing here.

The main thing was that i created a dataset containing 1.2M images ! do you understand how crazy that is ? this was a pre-req for the upcoming CapStone project which will be to do object segmentation and also monocular depth estimation both at the same time.

</details>
