## Introduction to Image Classification with Convolution Neural Network.

In this article, I will explain what CNN-Convolution Neural Network is and explain in the next article how to build a simple image classification with it.


Neural Networks are used in various artificial intelligence works like image classification, computer vision, audio classification. They are different neural networks for different applications.  For example,
we have RNN-Recurrent Neural Network for Time Series data, Text data, Audio data, Convolution Neural Network for Image data. Here are I will be explaining what CNN is.


A Convolution neural network (CNN) is a neural network that has one or more convolutional layers and is used mainly for image processing, classification, segmentation. A convolution simply means sliding a filter over an input. Sliding filters over an input create feature maps that summarize the presence of features in the input.
Image classifications with CNN essentially take an input image, process it and classify it under certain categories.

## Uses of Convolution Neural Network(CNN)

- Computer Vision

   *Facial Recognition*: A convolution neural network is used in recognizing different faces be it human or animal. It identify each facial features regardless on the external factors like the pose, light etc

 *Scene Labelling*: Each pixel is labelled with the category of the object it belongs to in scene labelling.

 *Image Classification*: Compared with other methods CNNs achieve better classification accuracy on large scale datasets due to their capability of joint feature and classifier learning.

 *Human Pose Estimation*:  Human Pose Estimation is defined as the problem of localization of human joints (also known as keypoints - elbows, wrists, etc) in images or videos. 

 *Document Analysis*: Document Analysis is the automatic extraction of information presented on paper and initially addressed to human comprehension. The output of Document analysis is a suitable symbolic representation that can be processed by computers.
![using cnn.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1615910291975/6U2D2yvOa.jpeg)

- Natural Language Processing

   *Speech recognition*: Speech recognition is the process of converting human sound signals into words or instructions.

![speech2.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1615911483344/ZJXiplIzC.png)

## Convolution Layers

### Input Layer
This layer takes in the raw input of an image with a certain dimension of width, height and depth.

### Convolution Layer
This layer extract features from the input image. It computes the dot product between all filters and image patch. suppose we have an image of dimension (  h * w* d) and a filter of dimension (fh*fw*Fd) then the convolution layer will output a volume of (h-fh+1)*(w-fw+1)*1.
Convolution of an image with different filters can perform operations such as edge detection, blur and sharpen by applying filters. The below example shows various convolution image after applying different types of filters (Kernels).

![conv.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1615911683441/oiZJ74bj8.png)


### Activation Function Layer 
This layer will apply activation functions to the output of the convolution layer. It is also referred to as non-linearity. Examples of the activation functions applied are Relu, Sigmoid, Tanh,  leaky Relu.
The volume remains unchanged.

### Pool Layer
Pooling is used to reduce the number of parameters when the image dimension is large. It is used periodically. It also prevents overfitting. The three common types of pooling are Max Pooling, Average Pooling, Sum Pooling.
In Max Pooling, the largest element from the rectified feature map is used.
![MaxpoolSample2.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1615726216289/TmPMXj7nZ.png)
In Average Pooling, the average of the elements in the feature map is used.

![gt.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1615726385645/IQStXM_dq.png)
 In Sum pooling, the sum of all elements in the feature map is used
 
### Fully-Connected Layer 
This layer takes input from the previous layer and computes the class scores and outputs the 1-D array of size equal to the number of classes.

##  Popular Architectures in Convolution Neural Networks
In practice, a Convolutional Neural Network is not created from scratch to solve problems: the most effective strategy is to take an existing network(An architecture) that classifies well a large collection of images (such as ImageNet) and apply Transfer Learning.
1. LeNet-5
2. AlexNet
3. VGG 16
4. Inception(GoogLeNet)
5. ResNet
6. ResNeXt
7. DenseNet

## Summary:
In this article, We learnt 
1. What a convolution neural network is.
2. The various uses of convolution network
3. The layers used when building a convolution neural network and 
4. The various architecture used in convolution neural network.




## References: 

http://cs231n.stanford.edu/

https://medium.com/@RaghavPrabhu/understanding-of-convolutional-neural-network-cnn-deep-learning-99760835f148


For a hands-on experience, the article below shows you a guide  :
https://neptune.ai/blog/neural-network-guide


