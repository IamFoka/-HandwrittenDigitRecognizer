# -HandwrittenDigitRecognizer
A handwritten digit recognizer that use a Convolutional Neural Network, written on python, ans trained with the MNIST dataset.

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
## How to use

 1-Using Jupyter, open the .ipynb file.

 2-The Jupyter's notebook codes are separated by cells, that can be executed apart.

 3-The first cell contains the import commands of all librarys (and the MNIST dataset) that we'll use and some configurations about the    input data. Also contains the model of our ConvNet, called "batata". When executed (the cell can be executed by pressing the "Run"      button, at the top of your screen), the block will build the model, and print all the model proprietaries. 

 4-The second cell's only made for the training, where the things such as the epochs quantity are inputted. Execute that, and the          train'll start. Using an i5-2320 it take 5 min/epoch. The "acc" represents the accuracy (0,1 = 10%).
   (you can see what happens here: http://prntscr.com/k13hka)

 5-On the third cell it's where the results are printed. The results come from the tests on all th 10000 images from the MNIST database.

 6-You can use the fourth cell to import a png image from your computer, and test the ConvNet on your own handwritten digit.

