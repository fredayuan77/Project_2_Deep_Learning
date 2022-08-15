# Project 2- Deep Learning: “Good Guys” vs. “Bad Guys” Image Classification 
*By Freda Qifei Yuan*

## Description
### Research Question
This project aims to develop appropriate Deep Learning models to classify facial images into the "Good Guys" and "Bad Guys". The category is defined by the likelihood to commit crimes and engage in violent behaviors. The "Bad/ unsavory" individuals have high tendency of being "convicted felons." By comparison, "Good/ savory" individuals are more likely to be "ordinary" people who follow the laws.


### Dataset: 

1. Data source: 12420 images in RGB format. Gerry Piosenka (2022, March). Good Guys-Bad Guys Image Data Set, Version 1. Retrieved May 7, 2022. [Data Link](https://www.kaggle.com/datasets/gpiosenka/good-guysbad-guys-image-data-set)

2. Feature: The dataset is a diverse image portfolio of age, sex, and race. In addition to biological facial traits, the samples also contain various emotions, with the most common being a smile face. Other individual identifier is also included, such as "glasses vs. no glasses", "long hair vs. short hair" ; "beard" vs. "no beard." These features could be recognized by the deep learning models as potential classifiers.

3. Target: binary classification outcome. The output = 0 is "savory", and = 1 is "unsavory."


## Methodology: 
-	Developed 6 variations of deep learning models using Python Keras. These models include both transfer learning and non-transfer learning. Specific structures include simple CNN, SqueezeNet, ResNet 50, and EfficientNet. 
-	Evaluated model performance by training& validation loss and accuracy metrics. 
- Selected best fit model for this project and explained reasons for best performance.

## Conclusion: 
- Based on validation accuracy and loss, EfficientNet achieves the highest performance. Among all six models, it has the highest training accuracy of 0.97 and highest validation score of above 0.94. 
- Reasons for Best Fit:
  1. This is a transfer learning model pretrained on ImageNet. I could use weights that are already calibrated to make image classification of this type. In other words, the model has already efficiently learned to extract features from human facial images in order to perform well on this related task.
  2. EfficientNet itself is a high performance architecture for image classification problem. CNN could be scaled up for better accuracy if more resources are available. Thus, by carefully balancing network depth, width, and resolution, a model can lead to better performance. 
