# MNIST_resizer
1. Resizing(make it smaller) MNIST to desired size of H x W, for desired number of training and test examples
2. Provides driver bit sequence for each input pixels of the new size. To be used for on-chip training

    Inputs:
        h = desired hight
        w = desired width
        numXtrain = number of training samples, subsample size(any value <=60000) 
        numXtest = number of testing samples(any value <=10000)
     
    Outputs
        Xtrain/x_in***.txt files, to drive input layer, #h*w driver files, each with numXtrain bit sequences
        XTest/x_in***.txt files, to drive input layer, #h*w driver files, each with numXtest bit sequences
