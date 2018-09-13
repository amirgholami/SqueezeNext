# SqueezeNext

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


# Other Frameworks
- For TensorFlow implementation, please see [Timen](https://github.com/Timen/squeezenext-tensorflow)'s implementation
- For Pytorch implementation, please see [osmr](https://github.com/osmr/imgclsmob)'s implementation

# Cifar-10/100, Tiny ImageNet
- For results on these datasets, please see [luuuyi](https://github.com/luuuyi/SqueezeNext.PyTorch)'s repository
