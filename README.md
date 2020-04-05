![GitHub Logo](satellite_pic)
Format: ![Alt Text](url)


Created by Olga Sutyrina, Sarah Elemili, Abduragim Shtanchaev and Artur Bille

# Individual Tree Crown classification on WorldView-2 Images using Autoencoder -- Group 9 Weak learners - Final Project (Machine Learning 2020 Course)
We analyzed sparse and convolutational autoencoders (SAE, CAE) with appended "classical" classifiers (AdaBoost, CatBoost, XGB, SVC, RFC, Log. Regr.), as well two convolutional neural networks (CNN) with different structures as end-to-end classifiers.
Details and explicit architectures of the considered models can found in the report. 

# Dependencies
Requirement:
* Python 3 with: 
  * Numpy
  * Matplotlib
  * rasterio
  * xgboost
  * torch
  * sklearn
  
To extract the pixels around a given tree, use our [*extractor*-module](https://github.com/arturbille/ML-project-Group9-WeakLearners/tree/master/Extractor).

# Installation
To run our codes you have to install the following modules: 
[fiona](https://pypi.org/project/Fiona/), [rasterio](https://rasterio.readthedocs.io/en/latest/) and [catboost](https://catboost.ai/docs/concepts/python-reference_apply_catboost_model.html)

# Data set
Our data set consists of three parts. The first one contains the whole satellite picture with 4561 x 6559 pixels and 8 channels. The second one includes 1012 labeled trees positions. Possible labels are: 0 = 'Spruce', 1 = 'Birch', 2 = 'Fir', 3 = 'Pine'. In the third part one can find positions of 10492 unlabeled tree crown positions within the satellite picture. The provided extractor module includes a function which extracts the pixels in the surrounding of every tree crown. 

# Usage
In this project we set up four experiments. To find all needed implemenations and results of each of them, follow this structure: 

1.  Autoencoders (AE) + 'classical' classifiers:

  * Convolutional autoencoder (CAE) -> [here](https://github.com/arturbille/ML-project-Group9-WeakLearners/tree/master/Models%20Implementation%20and%20Results/Autoencoder%20CAE-ABD%20-ML)
  
  * Sparse autoencoder (SAE) -> [here](https://github.com/arturbille/ML-project-Group9-WeakLearners/tree/master/Models%20Implementation%20and%20Results/Autoencoder%20SAE%20-AB)

2. Convolutional neural network (CNN):

  * 2D-CNN -> [here](https://github.com/arturbille/ML-project-Group9-WeakLearners/tree/master/Models%20Implementation%20and%20Results/2D-CNN%20Sarah)
  
  * VGG-CNN -> [here](https://github.com/arturbille/ML-project-Group9-WeakLearners/tree/master/Models%20Implementation%20and%20Results/VGG-CNN-Olya)

