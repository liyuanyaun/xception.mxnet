# A MXNet implementation of Xception

This is a [MXNet](http://mxnet.io/) implementation of Xception archetecture as described in the paper [Xception: Deep Learning with Depthwise Separable Convolutions](http://openaccess.thecvf.com/content_cvpr_2017/papers/Chollet_Xception_Deep_Learning_CVPR_2017_paper.pdf) by François Chollet at CVPR 2017.

The author's keras implementation can be found in the [https://github.com/fchollet/keras/tree/master/keras/applications](https://github.com/fchollet/keras/blob/master/keras/applications/xception.py) repo on GitHub.

This MXNet implementation is based on François Chollet's keras version. Furthermore, I also refered one implementation from [https://github.com/u1234x1234/mxnet-xception], but my version is more compact. I also attach the training code if you want train your own data with Xception archetecuture by yourself. Of course, if you just want to use the pretrained model by keras with MXNet, you can refer the python code from [https://github.com/u1234x1234/mxnet-xception/blob/master/keras2mxnet.py].

In original paper, author deploys Xception on 60 NVIDIA K80 GPUs for training ImageNet dataset. The ImageNet experiments took approximately 3 days. However, I only have 4 GPUs. I'm afraid the computational effiency on MXNet. I'm not sure whether MXNet has any optimization for depthwise separable convolution or not. 

#Requirements

Install MXNet on a mechine with CUDA GPU, and it's better also installed with [cuDNN v5](https://developer.nvidia.com/cudnn).

#Data

ImageNet'12 dataset

Imagenet 1000 class dataset with 1.2 million images. Because this dataset is about 120GB, so you have to download by yourself. Sorry for this inconvenience.

#How to Train





