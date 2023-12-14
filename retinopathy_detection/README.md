# kaggle competition

- https://www.kaggle.com/competitions/classroom-diabetic-retinopathy-detection-competition/overview

# Description
General information on the task:
Diabetic retinopathy is a common eye disease affecting more than 93 M people worldwide and notorious for being one of the major causes of blindness in the working-age population of the developed world. Scientists distinguish 4 stages of the disease differing in their symptoms and influence on human health. Progression to vision impairment can be slowed or even averted if diabetic retinopathy is detected in time. However, this can be difficult as the disease often shows few symptoms (stages 1, 2) until it is too late to provide effective treatment (stage 4). Currently, detecting diabetic retinopathy is a time-consuming and manual process that requires a trained clinician to examine and evaluate digital color fundus photos of the retina.

In 2015, EyePACs and California Healthcare Foundation organized a competition among data scientists on Kaggle platform. The competition was aimed at creating a model capable of identifying diabetic retinopathy stage given a color fundus photography as input. To evaluate the quality of the model, a metric called quadratic weighted kappa was suggested. Quadratic weighted kappa measures correlation between predicted and correct values. The more random the prediction is, the closer kappa is to zero. In contrast, the stronger the positive correlation is, the closer kappa is to unit. Top-10 participants were able to achieve kappa greater than 0.8, the level of performance comparable with that of clinician.

Inspired by the results of this competition, we decided to propose you a similar task as your 2 assignment.

# Objectives:
Create a convolutional neural network that takes color fundus images as input and predicts the stage of diabetic retinopathy on them.
Assignment will be considered as successfully completed if either quadratic weighted kappa for predictions of your model on test dataset is greater than 0.35 or your results are in TOP-40% of the classroom final rating
Datasets:
With the consent of EyePACs, this assignment uses preprocessed images of color fundus from Kaggle competition datasets. Preprocessing includes blurring, cropping, and resizing to 512x512. To prevent students from augmenting their training set by publicly available Kaggle test dataset, some color distortions were introduced to the images. These distortions cause funny changes in color palitra, but do not affect training efficiency. Numbers in filenames are ids of people. Left and Right mean left and right eyes (usually there is a strong correlation between stages of two eyes)

Training dataset consists of 35126 images each of which is assigned to one of 5 classes (0 class means a healthy eye). We have already divided training dataset into train and validation parts, but feel free to make your own division.
Test dataset is composed of 53576 not classified images
## Evaluation
Quadratic weighted kappa on test dataset