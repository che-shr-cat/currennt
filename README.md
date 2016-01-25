СURRENNT -- CUDA-enabled machine learning library for recurrent neural networks
================

### Authors

This is the fork of the CURRENNT library developed by Felix Weninger, Johannes Bergmann, and Bjoern Schuller from Technische Universitat Munchen.

Original site is [CURRENNT at sourceforge](http://currennt.sourceforge.net/)

Original paper is [Introducing CURRENNT - the Munich Open-Source
CUDA RecurREnt Neural Network Toolkit](http://mediatum.ub.tum.de/doc/1238161/796312.pdf)

Original readme is in 'README' file here.

The fork is based on 0.2-RC1 version.

### Description

CURRENNT is a machine learning library for Recurrent Neural Networks (RNNs) which uses NVIDIA graphics cards to accelerate the computations.

The library implements uni- and bidirectional Long Short-Term Memory (LSTM) architectures and supports deep networks as well as very large data sets that do not fit into main memory.

### Features

* Uni- and bidirectional Long Short-Term Memory (LSTM) layers with forget gates and peepholes
* Feedforward layers with tanh, logistic sigmoid and softmax activation functions
* Deep neural network architectures supported
* Cached on-line learning from large data sets (training data does not need to fit in main memory)
* Reads training data from NetCDF files
* Gradient descent with momentum
* Supports on-line, batch and hybrid on-line/batch learning
* Minimization of cross-entropy and squared error objectives
* Supports regression and binary/multiclass classification tasks
* Training with input activation noise for improved generalization
* Autosave after each training epoch

### What's new in the fork?

The original code has problems with compiling in recent operating systems. I personally found some problems with compiling it on Ubuntu 15.10. Here these problems are fixed.

* Support for Boost 1.60
* Support for CUDA 7.0/7.5 (thanks to [James Lyons](http://www.jimblog.net/2015/10/installing-currennt-on-ubuntu-1404.html))

It would be nice to add CTC sopport to the library. This one [from Baidu](https://github.com/baidu-research/warp-ctc) seems to be useful.
