# Dataset For Monocular Depth Estimation and Segmentation

![GitHub top language](https://img.shields.io/github/languages/top/Shakil-1501/TSAI?label=Python)     ![Maintenance](https://img.shields.io/maintenance/yes/2020?logo=Github)       ![GitHub repo size](https://img.shields.io/github/repo-size/Shakil-1501/TSAI?logo=Github&logoColor=red)   ![GitHub last commit](https://img.shields.io/github/last-commit/Shakil-1501/TSAI)   ![GitHub contributors](https://img.shields.io/github/contributors/SHAKIL-1501/TSAI)

## Objective

Create a custom dataset for monocular depth estimation and segmentation simultaneously.

Since we do not have acccess to a depth camera ,we use a pretrained depth model to generate the depth maps which will be used as ground truth for our model.

## Dataset Samples

**Background**:

![bg001](https://user-images.githubusercontent.com/63920152/89711422-dc7a7480-d9a7-11ea-9f4f-39c307c723bc.jpg)
![bg035](https://user-images.githubusercontent.com/63920152/89711424-ddaba180-d9a7-11ea-9da7-7f2bed5251a1.jpg)
![bg042](https://user-images.githubusercontent.com/63920152/89711425-de443800-d9a7-11ea-91cd-d1c9039d9881.jpg)
![bg046](https://user-images.githubusercontent.com/63920152/89711428-de443800-d9a7-11ea-84c7-a9f34d639a31.jpg)
![bg051](https://user-images.githubusercontent.com/63920152/89711429-dedcce80-d9a7-11ea-9325-1e15b9b7467b.jpg)
![bg052](https://user-images.githubusercontent.com/63920152/89711430-df756500-d9a7-11ea-8d51-646cba51290d.jpg)
![bg056](https://user-images.githubusercontent.com/63920152/89711432-df756500-d9a7-11ea-921f-27f7089e83d2.jpg)
![bg068](https://user-images.githubusercontent.com/63920152/89711815-3f6d0b00-d9aa-11ea-9512-9bf766a37f03.jpg)


**Foreground**:

![fg001](https://user-images.githubusercontent.com/63920152/89711754-dd140a80-d9a9-11ea-8383-c014ef2a0d24.jpg)
![fg022](https://user-images.githubusercontent.com/63920152/89711756-deddce00-d9a9-11ea-8ccb-356807f2cc8f.jpg)
![fg038](https://user-images.githubusercontent.com/63920152/89711758-df766480-d9a9-11ea-9394-db1d9bc21abd.jpg)
![fg045](https://user-images.githubusercontent.com/63920152/89711759-e00efb00-d9a9-11ea-9298-a0cd5a29cd1b.jpg)
![fg046](https://user-images.githubusercontent.com/63920152/89711760-e0a79180-d9a9-11ea-8152-49c5f15ec519.jpg)
![fg051](https://user-images.githubusercontent.com/63920152/89711761-e1402800-d9a9-11ea-9ae0-b1d908c05cf5.jpg)
![fg063](https://user-images.githubusercontent.com/63920152/89711762-e1d8be80-d9a9-11ea-96a2-279c798773bd.jpg)
![fg093](https://user-images.githubusercontent.com/63920152/89711763-e2715500-d9a9-11ea-8476-4983bcce5c61.jpg)

**Foreground Mask**


![ms022](https://user-images.githubusercontent.com/63920152/89712286-89a3bb80-d9ad-11ea-9a07-998c53a37b7c.jpg)
![ms038](https://user-images.githubusercontent.com/63920152/89712287-8a3c5200-d9ad-11ea-9308-b0ddd660e647.jpg)
![ms045](https://user-images.githubusercontent.com/63920152/89712289-8ad4e880-d9ad-11ea-840b-d188c0013713.jpg)
![ms046](https://user-images.githubusercontent.com/63920152/89712290-8b6d7f00-d9ad-11ea-84c3-63cda182de43.jpg)
![ms051](https://user-images.githubusercontent.com/63920152/89712291-8b6d7f00-d9ad-11ea-8b45-77537f73fdb2.jpg)
![ms063](https://user-images.githubusercontent.com/63920152/89712292-8c061580-d9ad-11ea-9caf-d05017752c92.jpg)
![ms069](https://user-images.githubusercontent.com/63920152/89712293-8c9eac00-d9ad-11ea-876a-450f236e1073.jpg)
![ms093](https://user-images.githubusercontent.com/63920152/89712294-8c9eac00-d9ad-11ea-9118-18a27c9463ff.jpg)

**Foreground Background overlay**

![fg_bg42001](https://user-images.githubusercontent.com/63920152/89713224-f5892280-d9b3-11ea-9159-4a266276c086.jpg)
![fg_bg74035](https://user-images.githubusercontent.com/63920152/89713225-f6ba4f80-d9b3-11ea-8408-57e4bcff6934.jpg)
![fg_bg88042](https://user-images.githubusercontent.com/63920152/89713226-f752e600-d9b3-11ea-917b-2e37db1e13de.jpg)
![fg_bg90046](https://user-images.githubusercontent.com/63920152/89713228-f7eb7c80-d9b3-11ea-923c-2ecd49d6c234.jpg)
![fg_bg100051](https://user-images.githubusercontent.com/63920152/89713229-f8841300-d9b3-11ea-8841-d707bbf088a7.jpg)
![fg_bg124052](https://user-images.githubusercontent.com/63920152/89713230-f91ca980-d9b3-11ea-870b-ba124665bd75.jpg)
![fg_bg136056](https://user-images.githubusercontent.com/63920152/89713231-f9b54000-d9b3-11ea-832b-432195080ef1.jpg)
![fg_bg184068](https://user-images.githubusercontent.com/63920152/89713233-fa4dd680-d9b3-11ea-880e-09db634d303f.jpg)

**Foreground-Background Depth**

![fg_bg42001](https://user-images.githubusercontent.com/63920152/89717491-c505b080-d9d4-11ea-8ed8-bbe3a75b87df.jpg)
![fg_bg74035](https://user-images.githubusercontent.com/63920152/89717492-c636dd80-d9d4-11ea-9f28-0c372b14fb9a.jpg)
![fg_bg88042](https://user-images.githubusercontent.com/63920152/89717493-c6cf7400-d9d4-11ea-9e43-c16ef495785f.jpg)
![fg_bg90046](https://user-images.githubusercontent.com/63920152/89717494-c6cf7400-d9d4-11ea-9361-956048d66bbf.jpg)
![fg_bg100051](https://user-images.githubusercontent.com/63920152/89717495-c7680a80-d9d4-11ea-862b-549911f25586.jpg)
![fg_bg124052](https://user-images.githubusercontent.com/63920152/89717497-c800a100-d9d4-11ea-88ee-afad3ed74746.jpg)
![fg_bg136056](https://user-images.githubusercontent.com/63920152/89717498-c800a100-d9d4-11ea-96bb-7b93cf64544a.jpg)
![fg_bg184068](https://user-images.githubusercontent.com/63920152/89717499-c8993780-d9d4-11ea-83a7-e3dac1d49985.jpg)




**Foreground-Background Mask**

![fg_bg42001](https://user-images.githubusercontent.com/63920152/89717524-12821d80-d9d5-11ea-8b93-1607e99d8c89.jpg)
![fg_bg74035](https://user-images.githubusercontent.com/63920152/89717525-13b34a80-d9d5-11ea-93ee-784b1d050087.jpg)
![fg_bg88042](https://user-images.githubusercontent.com/63920152/89717526-144be100-d9d5-11ea-9966-6553306a6c92.jpg)
![fg_bg90046](https://user-images.githubusercontent.com/63920152/89717527-14e47780-d9d5-11ea-84ef-60714a4d51cc.jpg)
![fg_bg100051](https://user-images.githubusercontent.com/63920152/89717528-157d0e00-d9d5-11ea-9860-2ee989c76f46.jpg)
![fg_bg124052](https://user-images.githubusercontent.com/63920152/89717529-157d0e00-d9d5-11ea-8556-6590e7816490.jpg)
![fg_bg136056](https://user-images.githubusercontent.com/63920152/89717530-1615a480-d9d5-11ea-98b8-4677f4199066.jpg)
![fg_bg184068](https://user-images.githubusercontent.com/63920152/89717531-16ae3b00-d9d5-11ea-8a4e-9f7063f4f428.jpg)

## Dataset Creation

### Background

   - "Jungles(forest)" images
   - 100 images of Jungles downloaded from net
   - Each image was resized to 224*224
   - Image dimensions:(224,224,3)
   - Directory size:4.47 MB
   
 ### Foreground
 
   - Images of objects with transparent background
   - 100 images of different animal were downloaded from net
   - Image dimensions:(125,125,3)
   - Directory size:2.45 MB
   
  ### Foreground Mask
 
   - For evey foreground its corresponding mask was created
   - Using GIMP the foreground was filled with white and background was filled with black
   - Number of images:100
   - Image dimensions:(125,125,3)
   
   Source code:
   
   ```python
   for i in range(1,100):
        img = cv2.imread('C:/Users/shakil uz zaman/Desktop/foreground/fg0'+str(i)+'.jpg',0)
        ret,thresh1 = cv2.threshold(img,240,255,cv2.THRESH_BINARY_INV)
        cv2.imwrite('ms0'+str(i)+'.jpg',thresh1)
   ```
   
   ### Foreground Overlayed on Background
   
   - For each background
     - Overlay each foreground randomly 20 times over background
     - Flip the foreground and again overlay it randomly 20 times on background
   - Number of images: 100*100*2*20 = 400,000
   - Image dimension:(224,224,3)
   - Directory size: 4.2 GB
   
   Source code:
   
   ```python
   import cv2
import random

j = 0
for i in range(1,201):  
    if i>=1 and i<=9:  
        background = cv2.imread('C:/Users/shakil uz zaman/Downloads/fg125x125/fg125x125/fg00'+str(i)+'.jpg')  
    elif i>=10 and i<=99:  
        background = cv2.imread('C:/Users/shakil uz zaman/Downloads/fg125x125/fg125x125/fg0'+str(i)+'.jpg')  
    else:
        background = cv2.imread('C:/Users/shakil uz zaman/Downloads/fg125x125/fg125x125/fg'+str(i)+'.jpg')  


    for k in range(0,20):  
        for file in os.listdir('C:/Users/shakil uz zaman/Downloads/bg224x224/'):  
            foreground = cv2.imread('C:/Users/shakil uz zaman/Downloads/bg224x224/'+file)  
            b=random.randint(25,99)  
            c=random.randint(25,99)  
            rows,cols,channels = background.shape  
            roi = foreground[b:rows+b, c:cols+c ]  
            img2gray = cv2.cvtColor(background,cv2.COLOR_BGR2GRAY)  
            ret, mask = cv2.threshold(img2gray, 240, 255, cv2.THRESH_BINARY_INV)  
            mask_inv = cv2.bitwise_not(mask)  
            img1_bg = cv2.bitwise_and(roi,roi,mask = mask_inv)  
            img2_fg = cv2.bitwise_and(background,background,mask = mask)  
            dst = cv2.add(img1_bg,img2_fg)  
            foreground[b:rows+b, c:cols+c] = dst  
            globals()['j'] = globals()['j']+1  
            cv2.imwrite('Trial2/fg_bg'+str(globals()['j'])+'.jpg',foreground)
            
   ```        
   
   ### Depth Map images
   
   - For each Foreground overlayed on background its corresponding depth map was generated
   - A pretrained monecular depth estimation model DenseDepth was used to generate the depth maps
   - Number of images :400,000
   - Image dimensions:(224,224)
   
   ### Foreground overlayed on Background Mask
   
   - For each Foreground overlayed on background its corresponding mask was generated
   - The mask was created by pasting the foreground mask on a black image at the same position foreground was overlayed
   - Number of images : 400,000
   - Image dimensions: (224,224)
   
   ## Dataset Link
   
   - Link: xyz
   
   
   |Type      |Count|Size|
   | -------- | ---- | --- |
   |**Background** |100  |4.47MB|
   |**Foreground** |100 |2.45MB|
   |**Foreground Mask** |100 | do update|
   |**Foreground-Background** | 400,000 | do update|
   |**Foreground-Background Mask** | 400,000 | do update|
   |**Foreground-Background Depth** | 400,000 | do update|
   
   ## Resources
   
   - Code to overlay foreground on background:
     
   
