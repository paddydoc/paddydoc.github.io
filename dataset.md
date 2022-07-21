---
title: Paddy Doctor dataset
subtitle: A visual and infrared image dataset of paddy diseases and pests.
layout: page
show_sidebar: false
hide_hero: true
---

### Kaggle Competition
A subset of this dataset (10,407 annotated images) has been used in the Kaggle competition - 
**[https://www.kaggle.com/c/paddy-disease-classification/](https://www.kaggle.com/c/paddy-disease-classification/)**

Note: The final and complete dataset will be released after compeltition of the competition (by end of Auguest 2022).

### Data Collection and annotation
![Data collection Overview](./assets/img/Datacollection_overview2.png)

We collected visual and infrared images of paddy leaves from real paddy fields in a village near the Tirunelveli district of Tamilnadu, India. We used the CAT S62 Pro smartphone that has inbuilt support for capturing both RGB and infrared images of the scene together. Our initial dataset contained more than 30,000 images, but we carefully examined each sample and excluded the noisy, out of focus, and redundant images. After cleaning, we had 16,225 images. Next, we annotated each leaf image with the help of an agricultural officer into one of the 12 disease categories and healthy leaves. 

The annotated paddy diseases are Bacterial Leaf Blight (BLB), Bacterial Leaf Streak (BLS), Bacterial Panicle Blight (BPB), Black Stem Borer (BSB), Blast, Brown spot, Downy Mildew, Hispa, Leaf Roller, Tungro, White Stem Borer, Yellow Stem Borer, and Normal leaf.  Although the original images were 1080x1440 pixels, we transformed them into a low-resolution image of 480x640 pixels to facilitate the processing and development of models on desktop computers. This  paddy dataset contains 12 disease and 20 pest classes collected using visual and infrared cameras together. In addition to the visual and infrared images, we also manually collected additional metadata for each leaf image, such as the age and variety of the paddy crops.


### Paddy disease images

#### RGB Images
![RGB Diseases](./assets/img/RGB_disease_classes2.png)

#### IR Images
![IR Diseasaes](./assets/img/IR_disease_classes.png)

### Paddy pest images
![RGB Pests](./assets/img/RGBpests.png)

![IR Pests](./assets/img/irpests.png)

