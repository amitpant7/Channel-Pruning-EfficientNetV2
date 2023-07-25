# Channel-Pruning-EfficientNetV2
I pruned 88% of channels of efficientNetV2 using LAMP pruning resulting 14x sammler model, 2.5x faster in inference, 14x less parameters &amp; 2.5x fewer MACops. The loss on accuracy was somewhat 2% only.

After that I replaced all the SiLU and sigmoid layers with Hard Swish and Hardsigmoid as the model is to be deployed in FPGA.


Notebook: https://www.kaggle.com/code/amitpant7/channel-pruning-of-effficientnet-upto-88-cifar 
