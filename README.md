# Retinal-Disease-Classification

The world faces a severe shortage of trained eye care professionals. According to the WHO (2020), it is estimated that at least 2.2 billion people worldwide are affected by visual impairment. We aim to mitigate the impacts of  eye care professional scarcity by creating a multi-label retinal disease classification CNN-based model.

## Data

The image dataset can be found [here](https://www.kaggle.com/andrewmvd/retinal-disease-classification). It consists of 3200 fundus images with 46 diagnostic labels.

## System Overview

Our CNN-based multi-label classification model gets rescaled fixed sized input fundus images of 640 x 640. The architecture consists of four pairs of convolutional
layers where each layer is followed by a max-pooling layer and a dropout layer of probability 0.25. The fourth convolutional layer is followed by flatten and
dense layers with soft-max function to make prediction. We used ReLU as activation functions. The layers of our model can be seen below. 


![CNN Layers](https://user-images.githubusercontent.com/75216302/143999664-5500a620-0253-46e6-b1dc-0000dde56f0b.png)

## Results 

The model has an accuracy of 1.00. The output is the probabilities (0,1) of the diseases present in the fundus depicted in the input image as predicted by 
the model shown in descending order.

![Input and Output of X_test[100]](https://user-images.githubusercontent.com/75216302/143999996-c1c1ad42-e0c6-46bd-bd0f-bb573d4150a6.png)


## Built With

* [Pillow](https://github.com/python-pillow/Pillow) - Image processing and manipulation

* [Keras](https://github.com/keras-team/keras) - Modeling

## Credits

[Kanitnuch Kerdted](https://github.com/piamkerdted)

[Kotchakorn Bunamorn](https://github.com/IamFah)

Korapat Thongwattananon 

Pannaruj Viseskul

## Acknowledgements

https://towardsdatascience.com/journey-to-the-center-of-multi-label-classification-384c40229bff
