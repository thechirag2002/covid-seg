# covid-seg
## UNet based Covid-19 Radiography Segmentation

## About the Dataset
**COVID-19 CHEST X-RAY DATABASE**

A team of researchers from Qatar University, Doha, Qatar, and the University of Dhaka, Bangladesh along with their collaborators from Pakistan and Malaysia in collaboration with medical doctors have created a database of chest X-ray images for COVID-19 positive cases along with Normal and Viral Pneumonia images. This COVID-19, normal and other lung infection dataset is released in stages. In the first release we have released 219 COVID-19, 1341 normal and 1345 viral pneumonia chest X-ray (CXR) images. In the first update, we have increased the COVID-19 class to 1200 CXR images. In the 2nd update, we have increased the database to 3616 COVID-19 positive cases along with 10,192 Normal, 6012 Lung Opacity (Non-COVID lung infection) and 1345 Viral Pneumonia images and corresponding lung masks. We will continue to update this database as soon as we have new x-ray images for COVID-19 pneumonia patients.  


**COVID-19 data:**
-----------------------
COVID data are collected from different publicly accessible dataset, online sources and published papers.
- 2473 CXR images are collected from padchest dataset[1].
- 183 CXR images from a Germany medical school[2].
- 559 CXR image from SIRM, Github, Kaggle & Tweeter[3,4,5,6]
- 400 CXR images from another Github source[7].


### With this dataset, segmented image of covid-19 chest under radiography is obtained by forking fully connected ***UNet model*** to obtain a mask for the corresponding chest image.

<div style="display:flex list-style-type:none padding:15">
  - Chest image 
  <img src="https://github.com/thechirag2002/covid-seg/blob/e40248cdbd8ca13db27213bc27025958033ef974/images/chest-image.png" width="250" height="250"/>
  - Mask Image
  <img src="https://github.com/thechirag2002/covid-seg/blob/e40248cdbd8ca13db27213bc27025958033ef974/images/chest-mask.png" width="250" height="250"/>
</div>



## DICE COEFFICIENT SCORE
The Dice coefficient (also known as the Sørensen–Dice coefficient and F1 score) is defined as two times the area of the intersection of A and B, divided by the sum of the areas of A and B
```
Dice = 2 |A∩B| / (|A|+|B|) = 2 TP / (2 TP + FP + FN) (TP=True Positives, FP=False Positives, FN=False Negatives)
```


### The above Segmentation is done in 30 number of EPOCHS and performed the task with dice coefficient score of _96.28_
<img src="https://github.com/thechirag2002/covid-seg/blob/b6b899fefa7727b0454bdf1b8be02ef9290991df/images/curves.png" width="750" height="300"/>
