Created by Olga Sutyrina, Sarah Elemili, Abduragim Shtanchaev and Artur Bille

# ML-project-09: Weak learners
This work was part of the lecture "Machine Learning" at Skoltech, Moscow, in 2020. 
We analyzed sparse and convolutational autoencoders (SAE, CAE) with appended "classical" classifiers (AdaBoost, CatBoost, XGB, SVC, RFC, Log. Regr.), as well two convolutional neural networks (CNN) with different structures as end-to-end classifiers.
Details and explicit architectures of the considered models can found in the report. 

# Dependencies
To extract

# Installation
To run our codes you have to install the following modules: 
[fiona](https://pypi.org/project/Fiona/), [rasterio](https://rasterio.readthedocs.io/en/latest/) and [catboost](https://catboost.ai/docs/concepts/python-reference_apply_catboost_model.html)

# Data set
Our data set consists of three parts. The first one contains the whole satellite picture with 4561 x 6559 pixels and 8 channels. The second one includes 1012 labeled trees positions. Possible labels are: 0 = 'Spruce', 1 = 'Birch', 2 = 'Fir', 3 = 'Pine'. In the third part one can find positions of 10492 unlabeled tree crown positions within the satellite picture. The provided extractor module includes a function which extracts the pixels in the surrounding of every tree crown. 

# Usage

