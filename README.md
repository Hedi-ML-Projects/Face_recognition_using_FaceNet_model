# Face_recognition_using_FaceNet_model

The main goal of this project is to detect and recognize the faces of five characters from Schitt's creek TV show in any given image. I have used a dataset called Schitts_creek_5_characters created by one of my friends.
This dataset includes three folders: train, validation and test. Train and validation sets contain solo photos of the characters while the test set includes photos in which there are more than one character. 

I have broken this project into smaller steps:

1. Detect the faces in the image using the MTCNN(Multi-Task Cascaded Convolutional Neural Network) face detector

2. Feed each of the detected faces to FaceNet model to obtain the embeddings for that face. It outputs a 128 dimensional vector for each face. I have used a pre-tained FaceNet model implemented in kers provided by [Hiroki Taniai](https://github.com/nyoki-mtl/keras-facenet/blob/master/README.md).

3. Feed the 128-dimensional vector to an SVM classifier which determines the identity of the person
