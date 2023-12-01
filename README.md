# Digit recognition using deep learning

## Context
One of the most interesting tasks in deep learning is to recognize objects in natural scenes. The ability to process visual information using machine learning algorithms can be very useful as demonstrated in various applications.

The SVHN dataset contains over 600,000 labeled digits cropped from street-level photos. It is one of the most popular image recognition datasets. It has been used in neural networks created by Google to improve the map quality by automatically transcribing the address numbers from a patch of pixels. The transcribed number with a known street address helps pinpoint the location of the building it represents.

## Objective
The objective is to predict the number depicted inside the image by using Artificial or Fully Connected Feed Forward Neural Networks and Convolutional Neural Networks. I experimented with various models of each and finally select the one that is giving us the best performance.

## Dataset
I used a a subset of the original data to save some computation time. The dataset is provided as a .h5 file. The basic preprocessing steps have been applied on the dataset.

## Final Observations:

The total number of trainable parameters in the CNN model 1 were: 267,306

The total number of trainable parameters in the CNN model 2 were: 164,170

The first model is less complex than the second model because it has a lower number of trainable parameters.

The second cnn model has two dense layers more than the first cnn model. The second model has two additional batch normalization layers, two LeakyReLU layers, one max-pooling layer, and a dropout layer. The second model has more epochs than the first model.

The second cnn model has a greater accuracy, 90.52%, than the first model, 85.12%. The second cnn model has a smaller loss score, 0.49, than the first model, 0.86. The second model took more time, 2 seconds, to process one epoch than the first model, 1 second.

Considering that the first model performs better in the training data than in the validation data, I can conclude that the the first model is overfitting. Adding regularization and dropout layers, like the second model does, would help address this.
