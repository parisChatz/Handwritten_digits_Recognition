# Handwritten_digits_Recognition
Neural Netwrok Implementation to recognise hand-written digits 
In this project neural networks are used torecognize handwritten digits (from 0 to 9).

# DATA SET
Each training example is a 20 pixel by 20 pixel grayscale image of the digit. 
Each pixel is represented by a floating point number indicating the grayscale 
intensity atthat location. The 20 by 20 grid of pixels is “unrolled” into a 
400-dimensional vector. Each of these training examples becomes a single row 
in our data matrix X. This gives us a 5000 by 400 matrix X where every row is 
a training example for a handwritten digit image.
The second part of the training set is a 5000-dimensional vector y that
contains labels for the training set. To make things more compatible with
Octave/MATLAB indexing,the digit zero is mapped to the value ten. 
Therefore, a “0” digit is labeled as “10”, while the digits “1” to “9” are labeled 
as “1” to “9” in their natural order.

# NEURAL NETWORK
The neural network has 3 layers – an input layer, a hidden layer and an output layer.
Recall that our inputs are pixel values ofdigit images. 
Since the images are of size 20×20, this gives us 400 input layer
units (excluding the extra bias unit which always outputs +1).

# Random initialization
When training neural networks, it is important to randomly initialize the parameters 
for symmetry breaking. One effective strategy for random initialization 
is to randomly select values for Θ (l) uniformly in the range {-e,+e}
You should use e = 0.12. 2 This range of values ensures that the parameters
are kept small and makes the learning more efficient.
