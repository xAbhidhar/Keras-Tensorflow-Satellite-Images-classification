# Image-classification-using-keras
National Agricultural Imagery Program collects satellite imagery data across the whole of
the Continental United States. Sample image dataset taken from the entire data includes numerous landscapes like rural areas, urban areas, mountains, forest
patches, rivers, lakes farms, etc. covering the entire state of California. This project aims to analyze the dataset using neural networks to classify the images into
either of following class – barren land, forest, grassland and others.

## Problem Statement
Build a deep leaning model to classify the images taken from satellite into the following categories:
   -  Barren Land
   -  Forest
   -  Grassland
   -  Others

## Libraries Used
The following libraries are used:
   -  `Keras` for creating neural net with integration with TensorFlow.

   -  `TensorFlow` as a backend for Keras.

   -  `Pandas` for various operations related to data processing.

   -  `Numpy` for implementation of linear algebra

   -  `Matplotlib`  for visualization 

   -  `Skimage` for image processing


## Implementation
Sequential model has been implemented with fully connected (dense) layers. Activation function used is 'softmax'. Optimizer used is 'Adam'.

#### Dataset
The Data is originally collected under National Agriculture Imagery Program (https://catalog.data.gov/dataset?tags=naip). The size of the original dataset is ~65 TB. The data is in the form of uncompressed `Digital Ortho Quarter Quad Tiles (DOQQs)`. These are the GeotTIFF images corresponding to the United States Geological Survey (USGUS). The model is trained on as subset of these images. Images consists of 4 different bands - 
   - Red 
   - Green 
   - Blue 
   - Near Infrared

#### Input Data Format
Labels are encoded as one hot encoded vectors(1x4) for each class of the landmass. Every patch of image is normalized to the size of 28x28 pixels. The data is in 4 CSV files -
   - X_test_sat4.csv: 100,000 training images, 28x28 images each with 4 channels 
   - y_test_sat4.csv: 100,000 training labels, 1x4 one-hot encoded vectors 

#### Test Set
Test set size is 10% of the input data. The test set consists 1,000 images. 

#### Model Selection
The model selected is the Neural Network with fully connected layers. 

## Technologies & Tools used
 - Python 
 - Jupyter Notebook
 - PyCharm
 - Tensorflow
 - Keras

## Results










