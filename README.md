# yuYpOTrvBrzkHSgq-MonReader


MonReader is a new mobile document digitalization experience for the blind, for researchers and for everyone else in need for fully automatic, highly fast and high-quality document scanning in bulk. It is composed of a mobile app and all the user needs to do is flip pages and everything is handled by MonReader: it detects page flips from low-resolution camera preview and takes a high-resolution picture of the document, recognizing its corners and crops it accordingly, and it dewarps the cropped document to obtain a bird's eye view, sharpens the contrast between the text and the background and finally recognizes the text with formatting kept intact, being further corrected by MonReader's ML powered redactor.
The Goal of the project is to Predict if the page is being flipped using a single image.

#Data Description
Data is  collected as page flipping video from smart phones and labelled them as flipping and not flipping.
The videos are clipped  as short videos and labelled them as flipping or not flipping. The extracted frames are then saved to disk in a sequential order with the following naming structure: VideoID_FrameNumber.

Data is then given as images.

#Approach.
I used both Pytorch and Tensorflow  to build a Convolution Neural Network Model.The Pytorch model gave the best accuracy of 98.66 and 100% prediction on single images.
I also built a Vision Transformer model which gave an accuracy of 97.82 upon evaluation.Several evaluation methods are perfored and the accuracy metrics evaluated are  high and consistent. 

The models are in two  separate notebook files:Monreader which have the CNN models and VisionTransformer with transsformer model.

