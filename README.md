# Image-classification-using-keras
National Agricultural Imagery Program (NAIP) collects satellite imagery data across the whole of
the Continental United States. An average image is 6000x7000 pixels have size of about 200MB
each. The entire dataset is approx. 65 TeraBytes. Sample image dataset taken from the entire
65TB of data includes numerous landscapes like rural areas, urban areas, mountains, forest
patches, rivers, lakes farms, etc. covering the entire state of California. NAIP developed an
image labeling tool to uniformly label image patches belonging to a specific landmass. However,
the labelling by this tool was performed manually which consumed high manpower and labor
cost. This project aims to analyze the dataset using neural networks to classify the images into
either of following – barren land, forest, grassland and others.

## Problem Statement
Bulid a deep leaning model to classify the images taken from satellite into the following categories:
   -  Barren Land
   -  Forest
   -  Grassland
   -  Others

## 

## Implementation

#### Dataset
The Data is originally collected under National Agriculture Imagery Program (NAIP) (https://catalog.data.gov/dataset?tags=naip). The size of the original dataset is ~65 TB. The data is in the form of uncompressed `Digital Ortho Quarter Quad Tiles (DOQQs)`. These are the GeotTIFF images corresponding to the United States Geological Survey (USGUS). The model is trained on as subset of these images. Images consists of 4 different bands - 
   - Red 
   - Green 
   - Blue 
   - Near Infrared

#### Input Data Format
Labels are encoded as one hot encoded vectors(1x4) for each class of the landmass. Every patch of image is normalized to the size of 28x28 pixels. The data is in 4 CSV files -
   - X_train_sat4.csv: 400,000 training images, 28x28 images each with 4 channels 
   - y_train_sat4.csv: 400,000 training labels, 1x4 one-hot encoded vectors 
   - X_test_sat4.csv: 100,000 training images, 28x28 images each with 4 channels 
   - y_test_sat4.csv: 100,000 training labels, 1x4 one-hot encoded vectors 

#### Validation and Test Set

#### Model Selection

#### Training

#### Evaluation

#### Hyperparameter tuning

#### Prediction
   
## Evaluation

## Technologies & Tools used
 - Python 
 - Jupyter Notebook
 - PyCharm
 - Tensorflow
 - Keras

## Results










