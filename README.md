# Mitochondria segmentation

We got images from 5x5x5µm section taken from the CA1 hippocampus region of the brain, corresponding to a 1065x2048x1536 volume. 
The researchers have annotated mitochondria, so each image also got a corresponding mask image.
We will read these files into Python and use the TensorFlow package.

The image files are grayscale and binary, and we will read these files into Python and use the TensorFlow package.

We will classify our detected mitochondria using computer vision techniques such as Convolutional Neural Networks (CNN) and the architecture is known as U-NET.

The result will be a binary outcome (1 or 0). If we detect a mitochondria, the value will be 1, else it will be 0.

The goal of this classification is to learn a Network to automatically detect mitochondira. The performance of the model will then be evaluated with a Intersect over Union-score (IoU-score)


## Data
The data comes from the Kaggle challenge: "Z by HP Unlocked Challenge 3 - Signal Processing".
https://www.epfl.ch/labs/cvlab/data/data-em/

## The Task
The Challenge is to build a Machine Learning model that learns the features of mitochondira and can then detect/segment them automatically.

**Data Explorer**

We are going to have 2 different files
* training.tif 
  - These are a stack of the training images in Grayscale
* training_groundtruth.tif
  - mask images of the training images and are used as the ground truth

