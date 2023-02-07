# Crop_Prediction

A project based on a model built by Deep Learning Algorithm, Convolutional Neural Network which can be used to predict crops like wheat, maize, rice, sugarcane, etc. from images. 
The Dataset for the project can be accessed by the link :- https://drive.google.com/file/d/1v-nHlweQA1lVadwW2gBmMXiDaRMbWu6v/view?usp=share_link .
The main purpose of this project is to get a simple understanding of how the Convolutional Networks work ------>

![image](https://user-images.githubusercontent.com/96066261/216238056-7d1ce807-c5b2-4dec-a554-60846b978474.png)

With the help of the above diagram we can easily identify the layers made in the Convolutional Neural Networks and these are not restricted to just 1 or 5 layers, we can make n number of hidden layers for our model.


# Overview

The above project contains a dataset consisting of images with crops :- Jute, Maize, Rice, Sugarcane and Wheat where we have to predict which image belongs to which class. We also have a csv file containing the details of the classes. The images can be as follows:
![image](https://user-images.githubusercontent.com/96066261/217152230-9040ee4a-778e-4aae-8209-9eb56febcb95.png)               ![image](https://user-images.githubusercontent.com/96066261/217152303-f5569bab-10b0-4929-b256-6c5c27edfcf9.png)                ![image](https://user-images.githubusercontent.com/96066261/217152332-ae6d5388-f917-4b5c-b97c-4def0ec1c140.png)      ![image](https://user-images.githubusercontent.com/96066261/217152354-3d214e42-ff69-4af7-ab35-01e115f626ad.png)                       ![image](https://user-images.githubusercontent.com/96066261/217152366-8f5f965d-6bb9-46a0-888a-45e411ec8fb0.png)


Also we can see the intesity of the images by using grayscale from OpenCV and easily visualize it in the dataset via graphs. For example,
![image](https://user-images.githubusercontent.com/96066261/217152665-914c7e77-c6d6-46e0-95c9-319076ccbfe7.png)

Now as we know that a machine cannot recognize or work omn strings or any other values except numerical values. So, to overcome this hurdle LabelEncoders are used to give a unique numerical value to each class. These classes can be easily used in the Convolutional Neural Networks. 

The below code demonstrates the use of the Sequential. A CNN can be instantiated as a Sequential model because each layer has exactly one input and output and is stacked together to form the entire network. from tensorflow.keras.models import SequentialCNN = Sequential(). 

  ![image](https://user-images.githubusercontent.com/96066261/217157396-a9b7ad2d-e15a-42f5-8d41-12bce6f7c797.png)


In the above piece of code we have used a an input layer, one output layer and in between are the hidden layers. With these layers we find out the features for the recognition also known as feature extraction. Then these features are stored in a higher dimensional array i.e., the matrix. Furthermore this matrix us flattened and then we classify the features which have been extracted. This part is known as Classification.

We can also see that the model has been trained 10 times with the help of epochs. An epoch is when all the training data is used at once and is defined as the total number of iterations of all the training data in one cycle for training the machine learning model. 

Another way to define an epoch is the number of passes a training dataset takes around an algorithm. One pass is counted when the data set has done both forward and backward passes. 

The number of epochs is considered a hyperparameter. It defines the number of times the entire data set has to be worked through the learning algorithm.


At last we can see the Validation Accuracy and Training Accuracy graph, also the Validation Loss and the Training Loss graph.

![image](https://user-images.githubusercontent.com/96066261/217157870-1cfdf35a-86ac-47e1-b00a-5b3111c4d2dd.png)
