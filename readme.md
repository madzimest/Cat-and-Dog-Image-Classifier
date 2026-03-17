# Cat and Dog Image Classifier

[![TensorFlow 2.x](https://img.shields.io/badge/TensorFlow-2.x-orange)](https://www.tensorflow.org/)
[![Keras](https://img.shields.io/badge/Keras-2.x-red)](https://keras.io/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A convolutional neural network (CNN) built with TensorFlow/Keras to classify images of cats and dogs. This project was completed as part of the freeCodeCamp **Machine Learning with Python** curriculum, achieving over **70% accuracy** on the test set (well above the required 63%).

---

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Model Architecture](#model-architecture)
- [Results](#results)
- [Acknowledgements](#acknowledgements)
- [License](#license)

---

## Project Overview
The goal is to create a binary classifier that distinguishes between images of cats and dogs. The model is trained on a labeled dataset of 2000 images (1000 cats, 1000 dogs) and validated on 1000 images. Finally, it predicts on 50 unlabeled test images, and the predictions are compared with hidden ground truth to verify performance.

Key techniques used:
- **Data preprocessing**: Rescaling pixel values to [0, 1].
- **Data augmentation**: Random rotations, shifts, flips, and zooms to reduce overfitting.
- **CNN architecture**: Multiple convolutional and pooling layers followed by dense layers and dropout.
- **Training**: Adam optimizer, binary crossentropy loss, early stopping via callbacks.


## Dataset
The dataset is provided by freeCodeCamp.


- **Training set**: 2000 images (balanced).
- **Validation set**: 1000 images (balanced).
- **Test set**: 50 images (no labels provided initially).


## Requirements
- Python 3.7+
- TensorFlow 2.x
- NumPy
- Matplotlib
- Google Colab (recommended) or local Jupyter environment


## Installation

### Using Google Colab (Recommended)
1. Open the provided notebook link (or create a new notebook).
2. Copy the cells from the [notebook file](cat_dog_classifier.ipynb) into your Colab notebook.
3. Run all cells sequentially.

### Local Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/cat-dog-classifier.git
   cd cat-dog-classifier

pip install tensorflow numpy matplotlib


wget -q https://cdn.freecodecamp.org/project-data/cats-and-dogs/cats_and_dogs.zip
unzip -q cats_and_dogs.zip


jupyter notebook cat_dog_classifier.ipynb
