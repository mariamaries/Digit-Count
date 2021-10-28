# Digit-Count

## Description

The goal of this project is to predict the count of digits in an image. 

The dataset contains 5000 training images and 1000 testing images, each of size 100 × 100. These images are formed by placing 1 to 5 digits from the MNIST dataset onto a noisy background.  

The implementation uses two methods: 

The first method uses a model trained to classify images on the MNIST dataset. This model is then converted into a fully convolutional network to predict maps representing the probability of digits being present at that location. Without additional training, these maps are used for the final prediction. 

For the second method, a new convolutional network was created to directly predict the number of digits. Here, the effect of pretraining was investigated, in regards to accuracy:  

- tested the accuracy using only 20%, and then 50% of the dataset 

- trained two models, one having some pre-trained layers on the MNIST classification, where the other one has all the layers randomly initialized 
