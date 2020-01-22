# Stat441/841 Statistical Classification

An array of assignments practicing model-based classification techniques without the usage of built-in libraries such as Scikit-learn during the Fall 2018 assignment.


## Assignment One

0_1_2.mat contains 300 handwritten 0's, 1's and 2's images scanned rom postal envelopes. These images are stored in a 64 x 300 matrix, where each column of the matrix is an 8 x 8 greyscale image. Pixel intensities are between 0 to 1.

For this assignment we are tasked to:
1) Find the low-dimensional mapping by PCA, then plot them. 
2) Use FDA to map the data in 2-dimensional space
3) Use LDA and QDA to compute respective decision boundaries and plot them
4) Attempt to implement QDA based on euclidean distance between points and the mean of each class.

## Assignment Two

For this assignment we were tasked to

1) Fit a logistic regression to a matrix containing pixel values for a person's face.
2) Use backward propagation and plot various test and training results from a combination of weight decay coefficients and nodes

## Data Challenges

Both data challenges required submissions that were evaluated on the overall accuracy between the predicted label and the ground truth label. Any model can be developed to complete the task. 

The first data challenge was completed after building a convolutional neural network using TensorFlow 93% public score.

The second data challenge was completed using K nearest neighbors with 97% public score.

## Final Project

For the final project, we worked with Capsule networks which is a type of convolutional neural network that was motivated to address the lack of spatial awareness in neurons. We proposed to incorporate a supervised conditional random field (CRF) loss based on Tang et. al. (2018)'s CRF loss to convnets. This is a regularizer that was based on pixel affinity that we believe would be a good replacement for LaLonde Bagci (2018)'s regularizer on their model to perform semantic segmentation called SegCaps, which is used to regularize the learned embedding of the input space, but tossed away during the prediction phase.

While our algorithms did not converge to their final values due to a lack of epochs from limited computing resources, our network achieved a Jaccard index of 0.67 on the test image, which was an improvement from the original SegCaps network which achieved an index of 0.61.