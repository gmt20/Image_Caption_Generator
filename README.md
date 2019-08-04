# Image_Caption_Generator
This is the capstone project for advanced level Deep Learning course by HSE on Coursera.
The major part of the code was provided as assignment.
This is an  image-to-caption deep learning model that can produce descriptions for real world images. A pre-trained InceptionV3 model for CNN encoder and  its last hidden layer as an embedding were used.
Since the problem is to generate image captions, RNN text generator should be trained on image. I used  image features as an initial state for RNN instead of zeros and  transformed the image feature vector to RNN hidden state size by fully-connected layer.
During training the ground truth tokens were fed into the lstm to get predictions of next tokens.

The architecture:
![alt_text](https://github.com/gmt20/Image_Caption_Generator/blob/master/imag1.png)




This model was executed on random pictures from internet. The results are as displayed:
![alt_text](https://github.com/gmt20/Image_Caption_Generator/blob/master/imag2.png)




![alt_text](https://github.com/gmt20/Image_Caption_Generator/blob/master/imag3.png)


