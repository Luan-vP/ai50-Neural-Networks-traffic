Initial accuracy of around 0.1
Likely due to the convolution layer

The Kernel is also trained!!!!

Adding a second dense layer increased the accuracy immediately from 0.1ish to 0.9

Accuracy seems very variable on each run (starting values?)

Removing the dropout increased the accuracy almost immediately to 1.

The same is true with just increasing Convolution size, or just increasing pooling size. 

Second hidden layer also makes quite a big difference

Duplicated the convulution and pooling layers, didn't see an increase in performance until used a smaller pooll size on the first one, under the intuition to let a larger picture through. Then it performed better than having a single conv/pooling pair

It does better without the second pooling layer, intuition is more data to the neural network layers.