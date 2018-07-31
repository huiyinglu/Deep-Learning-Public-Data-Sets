# Deep-Learning-Public-Data-Sets
Deep Learning Projects using public datasets.

This repository contains the following projects:
1. dog_app.ipynb:
   This project implemented a dog breed classifier app/algorithm according to the image given. If the given image is a dog image, it 
   will predict the dog breed (from total 133 breed); if the given image is a human image, it will predict the ensembling dog breed; if
   the image is neither a dog image nor a human image, it will return with an error message. Please scroll down to the last cell to see
   the fun result! The project includes the following major steps: 1) Create a CNN (Convolutional Neural Network) from scrach, then make
   prediction. 2) Apply transfer learning by using VGG16 pre-ttrained ImageNet model inside Keras to create a new model (remove last 
   layer in the pre-trained model, and add one pooling layer, one output layer) to make prediction. 3) Apply transfer learning by using
   Xception pre-trained ImageNet model inside Keras to create a new model (remove last layer in the pre-trained model, and add one
   pooling layer, one output layer) to make prediction. The last model (Xception + transfer learning) achieves impressive test accuracy!
   Assigning breed to dogs from images is considered exceptionally challenging. Why? a) Even a human would have great difficulty in
   distinguishing between a Brittany and a Welsh Springer Spaniel. b) It is not difficult to find other dog breed pairs with minimal
   inter-class variation c) Likewise, recall that labradors come in yellow, chocolate, and black. The vision-based algorithm will have
   to conquer this high intra-class variation to determine how to classify all of these different shades as the same breed. The random
   guess will provide a correct answer roughly 1 in 133 times, which corresponds to an accuracy of less than 1%. 
   The architecture we choosed is based on Xception model, which is one of the pre-trained ImageNet models. It can recognized 1000
   different object categories. ImageNet has over 10 million images and contains a lot of dog images - so the Xception model has been
   trained with similar data (dog) as our data. The Xception model choosed here has good performance compared to other ImageNet pre-trained
   models, hence able to help us boosts the test accuracy! 

2. Titanic.ipynb:
   Use Titanic dataset from Kaggle for predicting survival/not survival of a passenger.
   Use Logistic Regression and DNN for solving the classification problem.
   More descriptions is in the top cell of the Jupyter Notebook.

3. bank_note.ipynb:
   Use public dataset for predicting a bank note authenticate/not authenticate.
   Use DNN and Random Forest for solving the classification problem.
   More descriptions is in the top cell of Jupyter Notebook.

4. MNIST_DNN.ipynb:
   Use public available MNIST dataset to predict hand-written digits
   USE DNN with different numbers of unit and layer and different model
   (Tensorflow graph session, Keras) to solve the multi-class classfication problem.
   More descriptions is in the top cell of Jupyter Notebook.
