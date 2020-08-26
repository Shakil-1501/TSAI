# Session : 6

![GitHub top language](https://img.shields.io/github/languages/top/Shakil-1501/TSAI?label=Python)     ![Maintenance](https://img.shields.io/maintenance/yes/2020?logo=Github)          ![GitHub last commit](https://img.shields.io/github/last-commit/Shakil-1501/TSAI)   ![GitHub contributors](https://img.shields.io/github/contributors/SHAKIL-1501/TSAI) ![GitHub](https://img.shields.io/github/license/SHAKIL-1501/TSAI)

## Objective

Take our 5th session code
- run your model for 25 epochs for each:
  - without L1/L2 with BN
  - without L1/L2 with GBN
  - with L1 with BN
  - with L1 with GBN
  - with L2 with BN
  - with L2 with GBN
  - with L1 and L2 with BN
  - with L1 and L2 with GBN
 
- We  will not be running your code 8 times manually . We need to be smarter and write a single loop or iterator to iterate through these conditions. 
- draw ONE graph to show the validation accuracy curves for all 8 jobs above. This graph must have proper legends and it should be clear what we are looking at. 
- draw ONE graph to show the loss change curves for all 8 jobs above. This graph must have proper legends and it should be clear what we are looking at. 
- find any 25 misclassified images for "without L1/L2 with BN" AND "without L1/L2 with GBN" model. We should be using the saved model from the above jobs. 
  and L2 models. We must show the actual and predicted class names.
- make all the images available on Github Readme page, so we can upload the images for your assignment (We can upload them somewhere else as well for add image url).

------------------Testing Accuracy Analysis -------------------


Testing Accuracy Analysis is devided into 3 Parts :

1. L1 with BN and L2 With BN
2. L1 with GBN and L2 with GBN
3. L1_L2 with GBN and L1_l2 with BN

1. L1 with BN after 7th epoch more oscillation 
   whereas 
   L2 With BN before 7th Epoch having more Oscillation.

2. L1 with GBN After every Two epoch we  can observe flucatation
   whereas
   L2 with GBN after 12th Epoch test accuracy is almost constant.

3. L1_L2 with GBN Most of the time it is oscillating and amongst of all , it is giving worst accuracy.
   whereas
   L1_l2 with BN has given better accuracy for most of the epoch compared with L1_L2 with GBN

  as well as L1_l2 with BN started with lower test accuracy and till reaching 25th Epoch gave better accuracy
  compared with L1_L2 with GBN
  
  you can check the images in github files.
  
  ![](https://github.com/Shakil-1501/TSAI/blob/master/S6/accuracy.png)


_---------------------------------------Loss Function Analysis -------------------------------

1.L1& L2 with BN fall is most steep among all.

2.L1 with BN has less oscillation than L2 with BN

3.L1 with GBN and L2 with GBN they both are eqivalent in all the epochs but L1 with GBN wins at the end with lower losses.

4. L1 & L2 with BN and GBN they both are showing initial higher losses but became almost constant with no much fluctuations after some epochs


  you can check the images in github files.
  
  ![](https://github.com/Shakil-1501/TSAI/blob/master/S6/losses.png)
  
 ## Authors INFO
   
   Email : md.shakiluzzaman@gmail.com
   
   -[![](https://github.com/jagatabhay/TSAI/blob/master/logo.png)](https://www.linkedin.com/in/md-shakiluzzaman-894707129/)
  
  
  
