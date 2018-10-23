# Image-classification-using-keras
National Agricultural Imagery NAIP Program collects satellite imagery data across the whole of
the Continental United States. Sample image dataset taken from the entire data includes numerous landscapes like rural areas, urban areas, mountains, forest
patches, rivers, lakes farms, etc. covering the entire state of California. This project aims to analyze the dataset using neural networks to classify the images into
either of following class – barren land, forest, grassland and other.

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

### Dataset
The Data is originally collected under National Agriculture Imagery Program (https://catalog.data.gov/dataset?tags=naip). The size of the original dataset is ~65 TB. The data is in the form of uncompressed `Digital Ortho Quarter Quad Tiles (DOQQs)`. These are the GeotTIFF images corresponding to the United States Geological Survey (USGUS). The model is trained on as subset of these images. Images consists of 4 different bands - 
   - Red 
   - Green 
   - Blue 
   - Near Infrared

### Input Data Format
Labels are encoded as one hot encoded vectors(1x4) for each class of the landmass. Every patch of image is normalized to the size of 28x28 pixels. The data is in 4 CSV files -
   - X_test_sat4.csv: 100,000 training images, 28x28 images each with 4 channels 
   - y_test_sat4.csv: 100,000 training labels, 1x4 one-hot encoded vectors 

### Test Set
Test set size is 10% of the input data which makes the test set consists 1,000 images. 

### Model Selection
Implented the sequential model of keras. The model selected is the Neural Network with fully connected layers.

### Implementation
 
Sequential model in Keras is a linear stack of layers. Sequential model could be created by passing a list of layer instances to the constructor. Initially, the model needs to know the type of input shape it should expect. To tell the model the input shape, the first layer in the Sequential model receives the information about the input shape. This could be done is the following ways:
   - Passing a parameter “input_shape” to the first layer
   - Some 2d layers like “Dense” support specifying the input shape with the argument “input_dim”
 
Prior to building the model, the learning process needs to be configured. This is done by the compile method. It receives the following three arguments:
   - Optimizer
   - Loss Function
   - Accuracy metrics

##### Optimization Function
- Optimization algorithms are used to minimize an Objective/Error function
- Mathematical function dependent on the Model’s parameters which are used in computing target values(Y) from the set of predictors(X) used in the model.
- Goal is to minimize loss

Types of optimization algorithms:
- First order optimization algorithms
- Second order optimization algorithms

##### What is Adam Optimizer?
Adam is the short form of the Adaptive Moment Estimation. This optimization method is one of many optimization methods used in neural networks. Adam optimization computes adaptive learning rates for every parameter. Like AdaDelta, it stores decaying average of past squared gradients but it also keeps an exponentially decaying average of past gradients M(t). 
 
Adam optimizer performs very good in practice and compares favorably to other adaptive learning algorithms as it converges very quickly. Apart from fast convergence, Adam also have a very fast learning speed and is very efficient. It also alleviates the problem like Vanishing learning rate, slow convergence rate, high variance in parameter update which usually lead to fluctuating loss function.

Adam stands for Adaptive Moment Estimation
Adam also keeps an exponentially decaying average of past gradients M(t)
- It converges very fast
- Learning speed of the Model is quiet Fast and efficient


## Technologies & Tools used
 - Python 
 - Jupyter Notebook
 - PyCharm
 - Tensorflow
 - Keras

## Results
Predicted the image with over 80 percent accuracy.









