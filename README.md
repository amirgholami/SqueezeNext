# SqueezeNext

![Block](img/sqnxt_block.png)


This repository contains the Caffe implementation of SqueezeNext.
Each directory contains the network definition along with the solver parameters used for
training. For visualizing each architecture you can use [netscope](http://ethereon.github.io/netscope/#/editor) ( you need to copy the train_val.prototxt files).
For details of each architecture please see this [paper](https://arxiv.org/abs/1803.10615).


The corresponding trained caffemodel files are also available [here](https://www.dropbox.com/sh/jpijswazbwk8opf/AADtPJdnEnFRMpkdD5qZdjTUa?dl=0).
All
networks were trained using [IntelCaffe](https://github.com/intelcaffe/caffe/)
on 32 Intel KNightsLanding (KNL) using the same hyper-parameters.  Fine-tuning
the hyper-parameters for each model may lead to better results. Our goal has been
to show the general trend but please contact us if you got new results.

# Pytorch and Tensorflow
Pretrained SqueezeNext models on ImageNet have been added to [imgclsmob](https://github.com/osmr/imgclsmob) repository. In Pytorch you can use the following command to load the pretrained network:

from pytorchcv.model_provider import get_model as ptcv_get_model
net = ptcv_get_model(“sqnxt23_w1”, pretrained=True)

Other possible options for the model are "sqnxt23_w3d2", "sqnxt23_w2", "sqnxt23v5_w1", "sqnxt23v5_w3d2", "sqnxt23v5_w2".
And this is the [link](https://github.com/osmr/imgclsmob/blob/master/pytorch/pytorchcv/models/squeezenext.py) for the corresponding network definition(s).

For TensorFlow instructions please see [this link](https://pypi.org/project/tensorflowcv/).

# Other Implementations
- For TensorFlow implementation, please see [Timen](https://github.com/Timen/squeezenext-tensorflow)'s implementation

# Cifar-10/100, Tiny ImageNet
- For results on these datasets, please see [luuuyi](https://github.com/luuuyi/SqueezeNext.PyTorch)'s repository

