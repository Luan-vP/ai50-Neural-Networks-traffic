The model had an initial accuracy of around 0.1, it was starting with a very small hidden layer of 5 neurons. 
I increased this to 128 and immediately saw a big increase up to 0.7.
Adding the a second layer increased the accuracy to about 0.9. 
I had a great revelation when I realised that the Kernel is also trained!

Accuracy seemeds very variable on each run which I assumed was dependent on the starting position. 
Removing the dropout layer after the hidden layers increased the accuracy immediately to 1, but I assume it is not as resilient to new data. 
I also tried duplicating the convolution and pooling layers, although I found a drop in accuracy. 
My intuition is that the pooling step reduces the amount of information entering the hidden layers, and so they are less able to learn from it. 
This was supported by the fact that decreasing the pooling size also led to an increase in the accuracy. This actually prompted me to remove the second pooling layer. 
