# Skin_Disease_Classifier
This document contains entire understanding of the model.
Model is built using Google Colaboratory in the beginning to benefit the Virtual GPU and optimize development of the model.
## Introduction
### Significance: 
The proposed project holds immense significance due to its potential to address
several critical issues in the field of skin disease diagnosis:
### Early Detection:
Machine learning algorithms can analyze skin images to detect subtle
changes that might not be easily noticeable to the naked eye. Early detection is crucial for
improving treatment outcomes and reducing the progression of diseases.
### Access to Healthcare: 
Especially in remote or underserved areas, individuals often lack access
to dermatologists. A ML-powered system can act as a preliminary screening tool, offering
timely guidance on whether a professional consultation is necessary.
### Reducing Misdiagnosis: 
Skin diseases often share visual similarities, leading to misdiagnosis.
ML algorithms, trained on large datasets, can learn to differentiate between these conditions
with a high degree of reducing errors.

## Project Overview:
We have used several layers in the model which provide Block-wise approach to detect and classify skin diseases. 
This contains several layers such as MaxPooling2D, Conv2D, Dense, Dropout, Flatten, and Batch Normalization.
This model works on FIVE types of Skin Disease Detection
Using analysis we have chosen the most common types of skin diseases in the region.
This model took us almost an year to be built with multiple collaborators in order to acheive a validation accuracy of 90%.
This model was tested on InceptionV3 and VDD based models which did not perform any better, infact it performed worse.
This has a custom CNN based model which has Block-wise approach through layers to detect and identify skin disease from an image.

## Data Collection & Preprocessing:
We have used two datasets and combined them and used FIVE Skin Diseases.
Using analysis we have chosen the most common types of skin diseases in the region, that are:
### DermNet (Kaggle)
### ISIC 2019 (IEEE)
These datasets were unclean and the performance of the model on this dataset were poor.
We manually cleaned both datasets for unclear images.
We chose to keep the number of images close between diseases.
### Duplicate Image Removal:
Identify and remove duplicate images from the dataset to ensure that each image is unique.
Duplicate images can skew the training process.
### Metadata Validation:
Validate and clean the metadata associated with the images. Ensure that patient information is
appropriately anonymized, and any confidential data is removed or obscured.
Handling Missing Data:
Address missing data issues by identifying images with incomplete metadata or corrupted files.
24
For missing metadata, if possible, retrieve or complete the necessary information from reliable
sources.
For missing or corrupted images, consider image reconstruction techniques or remove the
affected samples.
### Data Standardization:
Standardize image resolution to a common size to ensure uniformity in the dataset. Resizing
images to a consistent resolution (e.g., 124x124 pixels) is often necessary for model
compatibility.
### Color Normalization:
Normalize the colors of the images to mitigate variations caused by lighting conditions, camera
settings, and other factors. Techniques like histogram equalization or color channel
normalization can be applied.

## Model Building:
This model took us almost an year to be built with multiple collaborators in order to acheive a validation accuracy of 90%.
This model was tested on InceptionV3 and VDD based models which did not perform any better, infact it performed worse.
This has a custom CNN based model which has Block-wise approach through layers to detect and identify skin disease from an image.
### Libraries and Frameworks:>
#### Numpy
#### openCV
#### TensorFlow
#### Keras
#### Matplotlib
#### Seaborn
### IDE:
#### Google Colab
#### Jupyter Notebook

## Results
### Epochs.
![image](https://github.com/basitdest/Skin_Disease_Classifier/assets/135953286/0e77fce3-7feb-4f05-a678-50021d291d86)
### Accuracy and Loss Plotting:
![image](https://github.com/basitdest/Skin_Disease_Classifier/assets/135953286/bdc3271e-8d05-42f2-8a8c-1462100f4270)
### Color Bar/ Confusion Matrix:
![image](https://github.com/basitdest/Skin_Disease_Classifier/assets/135953286/2abc9dea-29da-4bad-88c9-754d44a2c73c)
### HeatMap
![image](https://github.com/basitdest/Skin_Disease_Classifier/assets/135953286/cbf1a700-f6c1-4a94-bff1-1d888601d411)
### Results compared with different Architectures:
![image](https://github.com/basitdest/Skin_Disease_Classifier/assets/135953286/0512367a-790e-4939-bcbf-22e99c25bf32)

## Deployment:
We have currently used Streamlit to execute the model for now.

## Real Time Testing:
![image](https://github.com/basitdest/Skin_Disease_Classifier/assets/135953286/7ff4c7c2-ee7f-434b-a7f5-e160aaf80781)
![image](https://github.com/basitdest/Skin_Disease_Classifier/assets/135953286/a7456120-6978-4084-b61e-8789be340323)
![image](https://github.com/basitdest/Skin_Disease_Classifier/assets/135953286/95414397-e573-41f1-8e40-3934e38c8783)



