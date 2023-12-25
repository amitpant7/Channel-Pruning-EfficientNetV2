# Channel-Pruning-EfficientNetV2

I pruned 88% of channels of efficientNetV2 using LAMP pruning resulting 14x sammler model, 2.5x faster in inference, 14x fewer parameters &amp; 2.5x fewer MACops. The loss on accuracy was somewhat 2% only.

After that I replaced all the SiLU and sigmoid layers with Hard Swish and Hardsigmoid as the model is to be deployed in FPGA.


Notebook: https://www.kaggle.com/code/amitpant7/channel-pruning-of-effficientnet-upto-88-cifar 



![pruning_improv_channel](https://github.com/amitpant7/Channel-Pruning-EfficientNetV2/assets/50907565/20a6952e-d1aa-42b0-a3af-77c58b046606)
Fig: : Efficiency Improvements after channel pruning
![image](https://github.com/amitpant7/Channel-Pruning-EfficientNetV2/assets/50907565/c02a2312-0064-4dd5-b21e-ee726706ea3c)


Through the application of channel-based LAMP, we achieved an impressive 88% 
reduction in channels within the EfficientNetV2 model. This transformation yielded a 
model that is not only 14 times smaller in size but also demonstrated a remarkable 2.5-
fold improvement in inference speed. Furthermore, it showcased a substantial reduction 
with 14 times fewer parameters and 2.5 times fewer MAC operations, all while 
incurring just a modest 2% decrease in accuracy. These outcomes not only underscore 
the effectiveness of channel pruning but also emphasize the exciting potential for the 
development of leaner and faster deep learning models that can be deployed in edge 
devices without significant sacrifices in performance.

Pruned Model : https://github.com/amitpant7/Channel-Pruning-EfficientNetV2/blob/main/EfficientnetV2_S_hswish87.pth

This was done as a part of a major project which involved pruning and quantizing efficientnetV2 and then implementing it on FPGA

### Further Work 
Quantization of Pruned Model: https://github.com/amitpant7/Quantizing-Efficientnetv2-using-Vitis-AI-Pytorch/tree/main 
