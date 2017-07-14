# NN
---
This is a python neural net module, adapted from a homework assignment I did in Risi Kondor's Machine Learning class at the University of Chicago. 

### Usage
To **initialize** a network, call:
`net = nn.Network(inDim,biases,hiddenDims,outDim,learningRate)`,
where:
* inDim is the number of input dimensions (eg, 20)
* biases is the number of input bias neurons (eg, 1)
* hiddenDims is a list of hidden layer neuron counts (eg, [10,5])
* outDim is the number of output dimensions (eg, 1)
* learningRate is the eta value in backpropagation (eg, .5)

To **train** a network, call:
`net.train(trainX,trainY,testX,testY,epochs)`,
where:
* trainX is a numpy array of training data (of size [n,inDim])
* trainY is a numpy array of training data (of size [n,outDim])
* testX is a numpy array of test data (of size [m,inDim])
* testY is a numpy array of test data (of size [m,outDim])
* epochs is the number of epochs to train over

To **predict** on a set of data, call:
`net.predict(testX)`,
where:
* testX is a numpy array of test data (of size [n,inDim])
