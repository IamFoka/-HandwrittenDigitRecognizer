# Handwritten Digit Recognizer
A handwritten digit recognizer that use a Convolutional Neural Network, written on python, and trained with the MNIST dataset.

## Getting Started
**First you'll need to install:**

[Python](https://www.python.org/downloads/)

[Anaconda](https://www.anaconda.com/download/) - It's a good environment to work with machine learning, especially with Tensorflow that we're going to use.  

OpenCV - A library for the development of applications in the Computer vision field.  
*using the Anaconda CMD*: `conda install -c conda-forge opencv`

Keras - Used to facilitate the creation of deep learning models on Theano and Tensorflow.  
`pip install keras`

[Tensorflow](https://www.tensorflow.org/install/) - Originally developed by researchers and engineers from the Google Brain team within Google’s AI organization, it comes with strong support for machine learning and deep learning.  

Jupyter - It's a web based interface that allows for rapid prototyping and sharing of data-related projects.  
Can be downloaded using the Anaconda Navigator.

Numpy  
`pip install numpy`

Matplotlab  
`pip install matplotlab`  

## How it works

   Convolutional Neural Networks (CNN) is most used to image recognition, like handwritten digits from the MNIST dataset. A CNN isn't that different of a Classic Neural Network, they both use interconnected neurons and weights to make decisions, based on padrons that the Network learn by herself during the training.
   But, the difference is that when the Network process the image, before all the make decision part, four procediments are aplied:
   
##### 1- The convolutional layer:
   That is the most important part of all the process, because it carries out the heaviest part of the computational processing. It's composed of a filter commonly called a "kernel", that is basically a little matrix, made of values that can be interpreted as weigths, and that values are multiplied by the image values, summed an then added to a new matrix. The metod works as the image below:
![screenshot_2](https://user-images.githubusercontent.com/40413290/42132088-22e14c2a-7ce7-11e8-887c-5fae5dbb5263.png)
   This "featured map" can be just one in between others, each one created by one different kernel. You can see the function working [here](https://www.youtube.com/watch?v=KiftWz544_8).

##### 2- Activation function:
   We add the activations functions for this purpose: to check the value produced by a neuron and decide whether outside connections should consider this neuron "fired", or "activated", or not.
   
##### 3- Pooling layer:
   The Pooling Layer function divides the image in "pools", areas with the size inputted by the developer, and take the higher value inside that pool, creating a new matrix with all that most "valueble" values. The metod works as the image below:
![screenshot_3](https://user-images.githubusercontent.com/40413290/42132300-a9ae184c-7ceb-11e8-8fc4-08d7be6fa8a1.png)

##### 4- Flatten function:
   The last step before the Classic Neural Network receive the input to make the decisions, is to turn the image matrix, that pass by the previous metods, into a vector. And just that's what this function does.
![screenshot_4](https://user-images.githubusercontent.com/40413290/42132411-afdacb32-7ced-11e8-9e87-d6bd3c683a6b.png)

##### That was just a simple resume about all the convolutional process, but you can read and learn more about it here:
   http://cs231n.github.io/convolutional-networks/
   http://www.wildml.com/2015/09/implementing-a-neural-network-from-scratch/
   http://neuralnetworksanddeeplearning.com/
   https://pt.linkedin.com/pulse/o-que-%C3%A9-um-rede-neural-convolucional-alex-fernandes-mansano
   https://machinelearningmastery.com/handwritten-digit-recognition-using-convolutional-neural-networks-python-keras/
   https://blog.luisfred.com.br/reconhecimento-de-escrita-manual-com-redes-neurais-convolucionais/
   https://github.com/mnielsen/neural-networks-and-deep-learning
   http://www.din.uem.br/ia/neurais/

## How to use

1- Using Jupyter, open the .ipynb file.

2- The Jupyter's notebook codes are separated by cells, that can be executed apart.

3- The first cell contains the import commands of all librarys (and the MNIST dataset) that we'll use and some configurations about the    input data. Also contains the model of our ConvNet, called "batata". When executed (the cell can be executed by pressing the "Run"      button, at the top of your screen), the cell will build the model, and print all the model proprietaries. 

4- The second cell's only made for the training, where things such as the epochs quantity are inputted. Execute that, and the          train'll start. Using an i5-2320 it take 5 min/epoch. The "acc" represents the accuracy (0,1 = 10%).
![screenshot_1](https://user-images.githubusercontent.com/40413290/42130327-ddac6b14-7cb7-11e8-9f1b-fb7cc5458651.png)


5- On the third cell it's where the results are printed. The results come from the tests on all th 10000 images from the MNIST database.

6- You can use the fourth cell to import a png image from your computer, and test the ConvNet on your own handwritten digit. Your image **must** be on the same folder as the notebook, and you need to substitute the "INSIRA_AQUI.png" by your image file name.

![screenshot_5](https://user-images.githubusercontent.com/40413290/42132490-30b900ba-7cef-11e8-8f28-8f6ad89b63ff.png)



