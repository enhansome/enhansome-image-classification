# Awesome - Image Classification with stars

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) ⭐ 503,008 | 🐛 106 | 📅 2026-09-02

A curated list of deep learning image classification papers and codes since 2014, Inspired by [awesome-object-detection](https://github.com/amusi/awesome-object-detection) ⭐ 7,506 | 🐛 7 | 📅 2022-12-17, [deep\_learning\_object\_detection](https://github.com/hoya012/deep_learning_object_detection) ⭐ 11,384 | 🐛 5 | 🌐 Python | 📅 2024-02-12 and [awesome-deep-learning-papers](https://github.com/terryum/awesome-deep-learning-papers) ⭐ 26,183 | 🐛 37 | 🌐 TeX | 📅 2024-01-18.

## Background

I believe image classification is a great start point before diving into other computer vision fields, espacially
for begginers who know nothing about deep learning. When I started to learn computer vision, I've made a lot of mistakes, I wish someone could have told me that which paper I should start with back then. There doesn't seem to have a repository to have a list of image classification papers like [deep\_learning\_object\_detection](https://github.com/hoya012/deep_learning_object_detection) ⭐ 11,384 | 🐛 5 | 🌐 Python | 📅 2024-02-12 until now. Therefore, I decided to make a repository
of a list of deep learning image classification papers and codes to help others. My personal advice for people who
know nothing about deep learning, try to start with vgg, then googlenet, resnet, feel free to continue reading other listed papers or switch to other fields after you are finished.

**Note: I also have a repository of pytorch implementation of some of the image classification networks, you can check out [here](https://github.com/weiaicunzai/pytorch-cifar100) ⭐ 4,776 | 🐛 59 | 🌐 Python | 📅 2024-07-15.**

## Performance Table

For simplicity reason, I only listed the best top1 and top5 accuracy on ImageNet from the papers. Note that this does not necessarily mean one network is better than another when the acc is higher, cause some networks are focused on reducing the model complexity instead of improving accuracy, or some papers only give the single crop results on ImageNet, but others give the model fusion or multicrop results.

* ConvNet: name of the covolution network
* ImageNet top1 acc: best top1 accuracy on ImageNet from the Paper
* ImageNet top5 acc: best top5 accuracy on ImageNet from the Paper
* Published In: which conference or journal the paper was published in.

|              ConvNet              | ImageNet top1 acc | ImageNet top5 acc |                                 Published In                                 |
| :-------------------------------: | :---------------: | :---------------: | :--------------------------------------------------------------------------: |
|                Vgg                |        76.3       |        93.2       |                                   ICLR2015                                   |
|             GoogleNet             |         -         |       93.33       |                                   CVPR2015                                   |
|             PReLU-nets            |         -         |       95.06       |                                   ICCV2015                                   |
|               ResNet              |         -         |       96.43       |                                   CVPR2015                                   |
|            PreActResNet           |        79.9       |        95.2       |                                   CVPR2016                                   |
|            Inceptionv3            |        82.8       |       96.42       |                                   CVPR2016                                   |
|            Inceptionv4            |        82.3       |        96.2       |                                   AAAI2016                                   |
|        Inception-ResNet-v2        |        82.4       |        96.3       |                                   AAAI2016                                   |
| Inceptionv4 + Inception-ResNet-v2 |        83.5       |       96.92       |                                   AAAI2016                                   |
|                RiR                |         -         |         -         |                               ICLR Workshop2016                              |
|      Stochastic Depth ResNet      |       78.02       |         -         |                                   ECCV2016                                   |
|                WRN                |        78.1       |       94.21       |                                   BMVC2016                                   |
|             SqueezeNet            |        60.4       |        82.5       | arXiv2017([rejected by ICLR2017](https://openreview.net/forum?id=S1xh5sYgx)) |
|               GeNet               |       72.13       |       90.26       |                                   ICCV2017                                   |
|              MetaQNN              |         -         |         -         |                                   ICLR2017                                   |
|             PyramidNet            |        80.8       |        95.3       |                                   CVPR2017                                   |
|              DenseNet             |        79.2       |       94.71       |                                   ECCV2017                                   |
|             FractalNet            |        75.8       |       92.61       |                                   ICLR2017                                   |
|              ResNext              |         -         |       96.97       |                                   CVPR2017                                   |
|               IGCV1               |       73.05       |       91.08       |                                   ICCV2017                                   |
|     Residual Attention Network    |        80.5       |        95.2       |                                   CVPR2017                                   |
|              Xception             |         79        |        94.5       |                                   CVPR2017                                   |
|             MobileNet             |        70.6       |         -         |                                   arXiv2017                                  |
|              PolyNet              |       82.64       |       96.55       |                                   CVPR2017                                   |
|                DPN                |         79        |        94.5       |                                   NIPS2017                                   |
|             Block-QNN             |        77.4       |       93.54       |                                   CVPR2018                                   |
|              CRU-Net              |        79.7       |        94.7       |                                   IJCAI2018                                  |
|                DLA                |        75.3       |         -         |                                   CVPR2018                                   |
|             ShuffleNet            |        75.3       |         -         |                                   CVPR2018                                   |
|            CondenseNet            |        73.8       |        91.7       |                                   CVPR2018                                   |
|               NasNet              |        82.7       |        96.2       |                                   CVPR2018                                   |
|            MobileNetV2            |        74.7       |         -         |                                   CVPR2018                                   |
|               IGCV2               |       70.07       |         -         |                                   CVPR2018                                   |
|                hier               |        79.7       |        94.8       |                                   ICLR2018                                   |
|              PNasNet              |        82.9       |        96.2       |                                   ECCV2018                                   |
|             AmoebaNet             |        83.9       |        96.6       |                                   AAAI2018                                   |
|               SENet               |         -         |       97.749      |                                   CVPR2018                                   |
|            ShuffleNetV2           |       81.44       |         -         |                                   ECCV2018                                   |
|                CBAM               |       79.93       |       94.41       |                                   ECCV2018                                   |
|               IGCV3               |        72.2       |         -         |                                   BMVC2018                                   |
|                BAM                |       77.56       |       93.71       |                                   BMVC2018                                   |
|              MnasNet              |       76.13       |       92.85       |                                   CVPR2018                                   |
|               SKNet               |       80.60       |         -         |                                   CVPR2019                                   |
|               DARTS               |        73.3       |        91.3       |                                   ICLR2019                                   |
|            ProxylessNAS           |        75.1       |        92.5       |                                   ICLR2019                                   |
|            MobileNetV3            |        75.2       |         -         |                                   CVPR2019                                   |
|              Res2Net              |        79.2       |       94.37       |                                   PAMI2019                                   |
|             LIP-ResNet            |       79.33       |        94.6       |                                   ICCV2019                                   |
|            EfficientNet           |        84.3       |        97.0       |                                   ICML2019                                   |
|             FixResNeXt            |        86.4       |        98.0       |                                   NIPS2019                                   |
|                BiT                |        87.5       |         -         |                                   ECCV2020                                   |
|        PSConv + ResNext101        |       80.502      |       95.276      |                                   ECCV2020                                   |
|            NoisyStudent           |        88.4       |        98.7       |                                   CVPR2020                                   |
|               RegNet              |        79.9       |         -         |                                   CVPR2020                                   |
|              GhostNet             |        75.7       |         -         |                                   CVPR2020                                   |
|                ViT                |       88.55       |         -         |                                   ICLR2021                                   |
|                DeiT               |        85.2       |         -         |                                   ICML2021                                   |
|                PVT                |        81.7       |         -         |                                   ICCV2021                                   |
|              T2T-Vit              |        83.3       |         -         |                                   ICCV2021                                   |
|              DeepVit              |        80.9       |         -         |                                   Arvix2021                                  |
|                ViL                |        83.7       |         -         |                                   ICCV2021                                   |
|                TNT                |        83.9       |         -         |                                   Arvix2021                                  |
|                CvT                |        87.7       |         -         |                                   ICCV2021                                   |
|                CViT               |        84.1       |         -         |                                   ICCV2021                                   |
|              Focal-T              |        84.0       |         -         |                                   NIPS2021                                   |
|               Twins               |        83.7       |         -         |                                   NIPS2021                                   |
|               PVTv2               |        81.7       |         -         |                                    CVM2022                                   |

## Papers\&Codes

### VGG

**Very Deep Convolutional Networks for Large-Scale Image Recognition.**
Karen Simonyan, Andrew Zisserman

* code: [torchvision : https://github.com/pytorch/vision/blob/master/torchvision/models/vgg.py](https://github.com/pytorch/vision/blob/master/torchvision/models/vgg.py) ⭐ 17,897 | 🐛 1,205 | 🌐 Python | 📅 2026-09-04
* code: [keras-applications : https://github.com/keras-team/keras-applications/blob/master/keras\_applications/vgg16.py](https://github.com/keras-team/keras-applications/blob/master/keras_applications/vgg16.py) ⚠️ Archived
* code: [keras-applications : https://github.com/keras-team/keras-applications/blob/master/keras\_applications/vgg19.py](https://github.com/keras-team/keras-applications/blob/master/keras_applications/vgg19.py) ⚠️ Archived
* pdf: <https://arxiv.org/abs/1409.1556>

### GoogleNet

**Going Deeper with Convolutions**
Christian Szegedy, Wei Liu, Yangqing Jia, Pierre Sermanet, Scott Reed, Dragomir Anguelov, Dumitru Erhan, Vincent Vanhoucke, Andrew Rabinovich

* code: [unofficial-tensorflow : https://github.com/conan7882/GoogLeNet-Inception](https://github.com/conan7882/GoogLeNet-Inception) ⭐ 297 | 🐛 5 | 🌐 Python | 📅 2020-03-11
* code: [unofficial-caffe : https://github.com/lim0606/caffe-googlenet-bn](https://github.com/lim0606/caffe-googlenet-bn) ⭐ 130 | 🐛 7 | 🌐 Shell | 📅 2017-01-10
* pdf: <https://arxiv.org/abs/1409.4842>

### PReLU-nets

**Delving Deep into Rectifiers: Surpassing Human-Level Performance on ImageNet Classification**
Kaiming He, Xiangyu Zhang, Shaoqing Ren, Jian Sun

* code: [unofficial-chainer : https://github.com/nutszebra/prelu\_net](https://github.com/nutszebra/prelu_net) ⭐ 11 | 🐛 1 | 🌐 Python | 📅 2017-02-02
* pdf: <https://arxiv.org/abs/1502.01852>

### ResNet

**Deep Residual Learning for Image Recognition**
Kaiming He, Xiangyu Zhang, Shaoqing Ren, Jian Sun

* code: [torchvision : https://github.com/pytorch/vision/blob/master/torchvision/models/resnet.py](https://github.com/pytorch/vision/blob/master/torchvision/models/resnet.py) ⭐ 17,897 | 🐛 1,205 | 🌐 Python | 📅 2026-09-04
* code: [facebook-torch : https://github.com/facebook/fb.resnet.torch](https://github.com/facebook/fb.resnet.torch) ⚠️ Archived
* code: [keras-applications : https://github.com/keras-team/keras-applications/blob/master/keras\_applications/resnet.py](https://github.com/keras-team/keras-applications/blob/master/keras_applications/resnet.py) ⚠️ Archived
* code: [unofficial-tensorflow : https://github.com/ry/tensorflow-resnet](https://github.com/ry/tensorflow-resnet) ⚠️ Archived
* code: [unofficial-keras : https://github.com/raghakot/keras-resnet](https://github.com/raghakot/keras-resnet) ⭐ 1,389 | 🐛 24 | 🌐 Python | 📅 2021-01-12
* pdf: <https://arxiv.org/abs/1512.03385>

### PreActResNet

**Identity Mappings in Deep Residual Networks**
Kaiming He, Xiangyu Zhang, Shaoqing Ren, Jian Sun

* code: [unoffical-pytorch : https://github.com/kuangliu/pytorch-cifar/blob/master/models/preact\_resnet.py](https://github.com/kuangliu/pytorch-cifar/blob/master/models/preact_resnet.py) ⭐ 6,426 | 🐛 106 | 🌐 Python | 📅 2023-02-24
* code: [facebook-torch : https://github.com/facebook/fb.resnet.torch/blob/master/models/preresnet.lua](https://github.com/facebook/fb.resnet.torch/blob/master/models/preresnet.lua) ⚠️ Archived
* code: [official : https://github.com/KaimingHe/resnet-1k-layers](https://github.com/KaimingHe/resnet-1k-layers) ⭐ 938 | 🐛 1 | 🌐 Lua | 📅 2017-05-24
* code: [unoffical-mxnet : https://github.com/tornadomeet/ResNet](https://github.com/tornadomeet/ResNet) ⭐ 573 | 🐛 19 | 🌐 Python | 📅 2018-03-04
* pdf: <https://arxiv.org/abs/1603.05027>

### Inceptionv3

**Rethinking the Inception Architecture for Computer Vision**
Christian Szegedy, Vincent Vanhoucke, Sergey Ioffe, Jonathon Shlens, Zbigniew Wojna

* code: [torchvision : https://github.com/pytorch/vision/blob/master/torchvision/models/inception.py](https://github.com/pytorch/vision/blob/master/torchvision/models/inception.py) ⭐ 17,897 | 🐛 1,205 | 🌐 Python | 📅 2026-09-04
* code: [keras-applications : https://github.com/keras-team/keras-applications/blob/master/keras\_applications/inception\_v3.py](https://github.com/keras-team/keras-applications/blob/master/keras_applications/inception_v3.py) ⚠️ Archived
* pdf: <https://arxiv.org/abs/1512.00567>

### Inceptionv4 && Inception-ResNetv2

**Inception-v4, Inception-ResNet and the Impact of Residual Connections on Learning**
Christian Szegedy, Sergey Ioffe, Vincent Vanhoucke, Alex Alemi

* code: [unofficial-keras : https://github.com/kentsommer/keras-inceptionV4](https://github.com/kentsommer/keras-inceptionV4) ⭐ 467 | 🐛 2 | 🌐 Python | 📅 2017-09-10
* code: [unofficial-keras : https://github.com/titu1994/Inception-v4](https://github.com/titu1994/Inception-v4) ⭐ 388 | 🐛 4 | 🌐 Python | 📅 2017-09-07
* code: [unofficial-keras : https://github.com/yuyang-huang/keras-inception-resnet-v2](https://github.com/yuyang-huang/keras-inception-resnet-v2) ⭐ 179 | 🐛 0 | 🌐 Python | 📅 2021-03-23
* pdf: <https://arxiv.org/abs/1602.07261>

### RiR

**Resnet in Resnet: Generalizing Residual Architectures**
Sasha Targ, Diogo Almeida, Kevin Lyman

* code: [unofficial-tensorflow : https://github.com/SunnerLi/RiR-Tensorflow](https://github.com/SunnerLi/RiR-Tensorflow) ⭐ 4 | 🐛 1 | 🌐 Python | 📅 2017-09-16
* code: [unofficial-chainer : https://github.com/nutszebra/resnet\_in\_resnet](https://github.com/nutszebra/resnet_in_resnet) ⭐ 3 | 🐛 0 | 🌐 Python | 📅 2017-01-19
* pdf: <https://arxiv.org/abs/1603.08029>

### Stochastic Depth ResNet

**Deep Networks with Stochastic Depth**
Gao Huang, Yu Sun, Zhuang Liu, Daniel Sedra, Kilian Weinberger

* code: [unofficial-torch : https://github.com/yueatsprograms/Stochastic\_Depth](https://github.com/yueatsprograms/Stochastic_Depth) ⭐ 480 | 🐛 1 | 🌐 Lua | 📅 2018-08-13
* code: [unofficial-keras : https://github.com/dblN/stochastic\_depth\_keras](https://github.com/dblN/stochastic_depth_keras) ⭐ 139 | 🐛 2 | 🌐 Python | 📅 2020-07-21
* code: [unofficial-chainer : https://github.com/yasunorikudo/chainer-ResDrop](https://github.com/yasunorikudo/chainer-ResDrop) ⭐ 40 | 🐛 1 | 🌐 Python | 📅 2016-04-11
* pdf: <https://arxiv.org/abs/1603.09382>

### WRN

**Wide Residual Networks**
Sergey Zagoruyko, Nikos Komodakis

* code: [official : https://github.com/szagoruyko/wide-residual-networks](https://github.com/szagoruyko/wide-residual-networks) ⭐ 1,315 | 🐛 24 | 🌐 Lua | 📅 2019-08-20
* code: [unofficial-pytorch : https://github.com/meliketoy/wide-resnet.pytorch](https://github.com/meliketoy/wide-resnet.pytorch) ⭐ 479 | 🐛 15 | 🌐 Python | 📅 2020-01-09
* code: [unofficial-pytorch : https://github.com/xternalz/WideResNet-pytorch](https://github.com/xternalz/WideResNet-pytorch) ⭐ 346 | 🐛 2 | 🌐 Python | 📅 2021-04-29
* code: [unofficial-keras : https://github.com/asmith26/wide\_resnets\_keras](https://github.com/asmith26/wide_resnets_keras) ⭐ 138 | 🐛 6 | 🌐 Python | 📅 2024-01-18
* pdf: <https://arxiv.org/abs/1605.07146>

### SqueezeNet

**SqueezeNet: AlexNet-level accuracy with 50x fewer parameters and <0.5MB model size**
Forrest N. Iandola, Song Han, Matthew W. Moskewicz, Khalid Ashraf, William J. Dally, Kurt Keutzer

* code: [torchvision : https://github.com/pytorch/vision/blob/master/torchvision/models/squeezenet.py](https://github.com/pytorch/vision/blob/master/torchvision/models/squeezenet.py) ⭐ 17,897 | 🐛 1,205 | 🌐 Python | 📅 2026-09-04
* code: [unofficial-caffe : https://github.com/DeepScale/SqueezeNet](https://github.com/DeepScale/SqueezeNet) ⭐ 2,218 | 🐛 7 | 📅 2018-07-09
* code: [unofficial-keras : https://github.com/rcmalli/keras-squeezenet](https://github.com/rcmalli/keras-squeezenet) ⭐ 405 | 🐛 21 | 🌐 Python | 📅 2023-02-24
* code: [unofficial-caffe : https://github.com/songhan/SqueezeNet-Residual](https://github.com/songhan/SqueezeNet-Residual) ⭐ 155 | 🐛 2 | 🌐 CSS | 📅 2019-03-15
* pdf: <https://arxiv.org/abs/1602.07360>

### GeNet

**Genetic CNN**
Lingxi Xie, Alan Yuille

* code: [unofficial-tensorflow : https://github.com/aqibsaeed/Genetic-CNN](https://github.com/aqibsaeed/Genetic-CNN) ⭐ 222 | 🐛 1 | 🌐 Python | 📅 2022-04-18
* pdf: <https://arxiv.org/abs/1703.01513>

### MetaQNN

**Designing Neural Network Architectures using Reinforcement Learning**
Bowen Baker, Otkrist Gupta, Nikhil Naik, Ramesh Raskar

* code: [official : https://github.com/bowenbaker/metaqnn](https://github.com/bowenbaker/metaqnn) ⭐ 139 | 🐛 2 | 🌐 Python | 📅 2017-07-18
* pdf: <https://arxiv.org/abs/1611.02167>

### PyramidNet

**Deep Pyramidal Residual Networks**
Dongyoon Han, Jiwhan Kim, Junmo Kim

* code: [unofficial-pytorch : https://github.com/dyhan0920/PyramidNet-PyTorch](https://github.com/dyhan0920/PyramidNet-PyTorch) ⭐ 270 | 🐛 0 | 🌐 Python | 📅 2020-07-05
* code: [official : https://github.com/jhkim89/PyramidNet](https://github.com/jhkim89/PyramidNet) ⭐ 131 | 🐛 0 | 🌐 Lua | 📅 2017-10-31
* pdf: <https://arxiv.org/abs/1610.02915>

### DenseNet

**Densely Connected Convolutional Networks**
Gao Huang, Zhuang Liu, Laurens van der Maaten, Kilian Q. Weinberger

* code: [official : https://github.com/liuzhuang13/DenseNet](https://github.com/liuzhuang13/DenseNet) ⭐ 4,870 | 🐛 30 | 🌐 Lua | 📅 2024-01-09
* code: [unofficial-pytorch : https://github.com/bamos/densenet.pytorch](https://github.com/bamos/densenet.pytorch) ⭐ 839 | 🐛 7 | 🌐 Python | 📅 2018-08-16
* code: [unofficial-keras : https://github.com/titu1994/DenseNet](https://github.com/titu1994/DenseNet) ⭐ 709 | 🐛 7 | 🌐 Python | 📅 2020-06-10
* code: [unofficial-keras : https://github.com/flyyufelix/DenseNet-Keras](https://github.com/flyyufelix/DenseNet-Keras) ⭐ 564 | 🐛 15 | 🌐 Python | 📅 2019-10-12
* code: [unofficial-tensorflow : https://github.com/YixuanLi/densenet-tensorflow](https://github.com/YixuanLi/densenet-tensorflow) ⭐ 563 | 🐛 10 | 🌐 Python | 📅 2019-05-07
* code: [unofficial-pytorch : https://github.com/YixuanLi/densenet-tensorflow](https://github.com/YixuanLi/densenet-tensorflow) ⭐ 563 | 🐛 10 | 🌐 Python | 📅 2019-05-07
* code: [unofficial-caffe : https://github.com/shicai/DenseNet-Caffe](https://github.com/shicai/DenseNet-Caffe) ⭐ 361 | 🐛 17 | 📅 2019-08-29
* pdf: <https://arxiv.org/abs/1608.06993>

### FractalNet

**FractalNet: Ultra-Deep Neural Networks without Residuals**
Gustav Larsson, Michael Maire, Gregory Shakhnarovich

* code: [unofficial-keras : https://github.com/snf/keras-fractalnet](https://github.com/snf/keras-fractalnet) ⭐ 156 | 🐛 0 | 🌐 Python | 📅 2017-09-17
* code: [unofficial-caffe : https://github.com/gustavla/fractalnet](https://github.com/gustavla/fractalnet) ⭐ 150 | 🐛 5 | 🌐 C++ | 📅 2017-10-11
* code: [unofficial-tensorflow : https://github.com/tensorpro/FractalNet](https://github.com/tensorpro/FractalNet) ⭐ 46 | 🐛 1 | 🌐 Python | 📅 2017-01-26
* pdf: <https://arxiv.org/abs/1605.07648>

### ResNext

**Aggregated Residual Transformations for Deep Neural Networks**
Saining Xie, Ross Girshick, Piotr Dollár, Zhuowen Tu, Kaiming He

* code: [keras-applications : https://github.com/keras-team/keras-applications/blob/master/keras\_applications/resnext.py](https://github.com/keras-team/keras-applications/blob/master/keras_applications/resnext.py) ⚠️ Archived
* code: [official : https://github.com/facebookresearch/ResNeXt](https://github.com/facebookresearch/ResNeXt) ⚠️ Archived
* code: [unofficial-pytorch : https://github.com/prlz77/ResNeXt.pytorch](https://github.com/prlz77/ResNeXt.pytorch) ⭐ 518 | 🐛 7 | 🌐 Python | 📅 2020-08-01
* code: [unofficial-keras : https://github.com/titu1994/Keras-ResNeXt](https://github.com/titu1994/Keras-ResNeXt) ⭐ 223 | 🐛 8 | 🌐 Python | 📅 2021-04-17
* code: [unofficial-tensorflow : https://github.com/taki0112/ResNeXt-Tensorflow](https://github.com/taki0112/ResNeXt-Tensorflow) ⭐ 158 | 🐛 4 | 🌐 Python | 📅 2018-08-14
* code: [unofficial-tensorflow : https://github.com/wenxinxu/ResNeXt-in-tensorflow](https://github.com/wenxinxu/ResNeXt-in-tensorflow) ⭐ 77 | 🐛 9 | 🌐 Python | 📅 2018-02-18
* pdf: <https://arxiv.org/abs/1611.05431>

### IGCV1

**Interleaved Group Convolutions for Deep Neural Networks**
Ting Zhang, Guo-Jun Qi, Bin Xiao, Jingdong Wang

* code [official : https://github.com/hellozting/InterleavedGroupConvolutions](https://github.com/hellozting/InterleavedGroupConvolutions) ⭐ 110 | 🐛 2 | 🌐 Python | 📅 2017-12-21
* pdf: <https://arxiv.org/abs/1707.02725>

### Residual Attention Network

**Residual Attention Network for Image Classification**
Fei Wang, Mengqing Jiang, Chen Qian, Shuo Yang, Cheng Li, Honggang Zhang, Xiaogang Wang, Xiaoou Tang

* code: [unofficial-pytorch : https://github.com/tengshaofeng/ResidualAttentionNetwork-pytorch](https://github.com/tengshaofeng/ResidualAttentionNetwork-pytorch) ⭐ 685 | 🐛 20 | 🌐 Python | 📅 2018-10-29
* code: [official : https://github.com/fwang91/residual-attention-network](https://github.com/fwang91/residual-attention-network) ⭐ 558 | 🐛 18 | 📅 2017-07-21
* code: [unofficial-gluon : https://github.com/PistonY/ResidualAttentionNetwork](https://github.com/PistonY/ResidualAttentionNetwork) ⭐ 107 | 🐛 1 | 🌐 Python | 📅 2019-06-12
* code: [unofficial-keras : https://github.com/koichiro11/residual-attention-network](https://github.com/koichiro11/residual-attention-network) ⭐ 92 | 🐛 7 | 🌐 Python | 📅 2018-04-16
* pdf: <https://arxiv.org/abs/1704.06904>

### Xception

**Xception: Deep Learning with Depthwise Separable Convolutions**
François Chollet

* code: [unofficial-pytorch : https://github.com/jfzhang95/pytorch-deeplab-xception/blob/master/modeling/backbone/xception.py](https://github.com/jfzhang95/pytorch-deeplab-xception/blob/master/modeling/backbone/xception.py) ⭐ 3,000 | 🐛 134 | 🌐 Python | 📅 2024-08-04
* code: [keras-applications : https://github.com/keras-team/keras-applications/blob/master/keras\_applications/xception.py](https://github.com/keras-team/keras-applications/blob/master/keras_applications/xception.py) ⚠️ Archived
* code: [unofficial-pytorch : https://github.com/tstandley/Xception-PyTorch](https://github.com/tstandley/Xception-PyTorch) ⭐ 264 | 🐛 0 | 🌐 Python | 📅 2023-01-16
* code: [unofficial-tensorflow : https://github.com/kwotsin/TensorFlow-Xception](https://github.com/kwotsin/TensorFlow-Xception) ⭐ 214 | 🐛 6 | 🌐 Python | 📅 2019-09-09
* code: [unofficial-caffe : https://github.com/yihui-he/Xception-caffe](https://github.com/yihui-he/Xception-caffe) ⭐ 46 | 🐛 3 | 📅 2024-05-02
* pdf: <https://arxiv.org/abs/1610.02357>

### MobileNet

**MobileNets: Efficient Convolutional Neural Networks for Mobile Vision Applications**
Andrew G. Howard, Menglong Zhu, Bo Chen, Dmitry Kalenichenko, Weijun Wang, Tobias Weyand, Marco Andreetto, Hartwig Adam

* code: [keras-applications : https://github.com/keras-team/keras-applications/blob/master/keras\_applications/mobilenet.py](https://github.com/keras-team/keras-applications/blob/master/keras_applications/mobilenet.py) ⚠️ Archived
* code: [unofficial-tensorflow : https://github.com/Zehaos/MobileNet](https://github.com/Zehaos/MobileNet) ⭐ 1,659 | 🐛 47 | 🌐 Python | 📅 2017-11-06
* code: [unofficial-caffe : https://github.com/shicai/MobileNet-Caffe](https://github.com/shicai/MobileNet-Caffe) ⭐ 1,273 | 🐛 48 | 🌐 Python | 📅 2021-06-08
* pdf: <https://arxiv.org/abs/1704.04861>
* code: [unofficial-pytorch : https://github.com/marvis/pytorch-mobilenet](https://github.com/marvis/pytorch-mobilenet)

### PolyNet

**PolyNet: A Pursuit of Structural Diversity in Very Deep Networks**
Xingcheng Zhang, Zhizhong Li, Chen Change Loy, Dahua Lin

* code: [official : https://github.com/open-mmlab/polynet](https://github.com/open-mmlab/polynet) ⭐ 80 | 🐛 4 | 📅 2017-07-23
* pdf: <https://arxiv.org/abs/1611.05725>

### DPN

**Dual Path Networks**
Yunpeng Chen, Jianan Li, Huaxin Xiao, Xiaojie Jin, Shuicheng Yan, Jiashi Feng

* code: [official : https://github.com/cypw/DPNs](https://github.com/cypw/DPNs) ⭐ 526 | 🐛 16 | 🌐 Python | 📅 2019-03-13
* code: [unofficial-pytorch : https://github.com/rwightman/pytorch-dpn-pretrained](https://github.com/rwightman/pytorch-dpn-pretrained) ⭐ 205 | 🐛 1 | 🌐 Python | 📅 2019-06-11
* code: [unoffical-keras : https://github.com/titu1994/Keras-DualPathNetworks](https://github.com/titu1994/Keras-DualPathNetworks) ⭐ 112 | 🐛 3 | 🌐 Python | 📅 2020-02-09
* code: [unofficial-pytorch : https://github.com/oyam/pytorch-DPNs](https://github.com/oyam/pytorch-DPNs) ⭐ 89 | 🐛 1 | 🌐 Python | 📅 2017-08-30
* pdf: <https://arxiv.org/abs/1707.01629>

### Block-QNN

**Practical Block-wise Neural Network Architecture Generation**
Zhao Zhong, Junjie Yan, Wei Wu, Jing Shao, Cheng-Lin Liu

* pdf: <https://arxiv.org/abs/1708.05552>

### CRU-Net

**Sharing Residual Units Through Collective Tensor Factorization in Deep Neural Networks**
Chen Yunpeng, Jin Xiaojie, Kang Bingyi, Feng Jiashi, Yan Shuicheng

* code [unofficial-mxnet : https://github.com/bruinxiong/Modified-CRUNet-and-Residual-Attention-Network.mxnet](https://github.com/bruinxiong/Modified-CRUNet-and-Residual-Attention-Network.mxnet) ⭐ 67 | 🐛 11 | 🌐 Python | 📅 2018-10-22
* code [official : https://github.com/cypw/CRU-Net](https://github.com/cypw/CRU-Net) ⭐ 45 | 🐛 5 | 📅 2017-04-14
* pdf: <https://arxiv.org/abs/1703.02180>

## DLA

**Deep Layer Aggregation**
Fisher Yu, Dequan Wang, Evan Shelhamer, Trevor Darrell

* code: [official-pytorch: https://github.com/ucbdrive/dla](https://github.com/ucbdrive/dla) ⭐ 440 | 🐛 17 | 🌐 Python | 📅 2022-01-04
* pdf: <https://arxiv.org/abs/1707.06484>

### ShuffleNet

**ShuffleNet: An Extremely Efficient Convolutional Neural Network for Mobile Devices**
Xiangyu Zhang, Xinyu Zhou, Mengxiao Lin, Jian Sun

* code: [unofficial-caffe : https://github.com/farmingyard/ShuffleNet](https://github.com/farmingyard/ShuffleNet) ⭐ 453 | 🐛 17 | 🌐 C++ | 📅 2018-08-30
* code: [unofficial-tensorflow : https://github.com/MG2033/ShuffleNet](https://github.com/MG2033/ShuffleNet) ⭐ 381 | 🐛 10 | 🌐 Python | 📅 2018-12-04
* code: [unofficial-pytorch : https://github.com/jaxony/ShuffleNet](https://github.com/jaxony/ShuffleNet) ⭐ 296 | 🐛 6 | 🌐 Python | 📅 2017-12-20
* code: [unofficial-keras : https://github.com/scheckmedia/keras-shufflenet](https://github.com/scheckmedia/keras-shufflenet) ⚠️ Archived
* pdf: <https://arxiv.org/abs/1707.01083>

### CondenseNet

**CondenseNet: An Efficient DenseNet using Learned Group Convolutions**
Gao Huang, Shichen Liu, Laurens van der Maaten, Kilian Q. Weinberger

* code: [official : https://github.com/ShichenLiu/CondenseNet](https://github.com/ShichenLiu/CondenseNet) ⭐ 690 | 🐛 11 | 🌐 Python | 📅 2019-11-11
* code: [unofficial-tensorflow : https://github.com/markdtw/condensenet-tensorflow](https://github.com/markdtw/condensenet-tensorflow) ⭐ 29 | 🐛 3 | 🌐 Python | 📅 2018-02-01
* pdf: <https://arxiv.org/abs/1711.09224>

### NasNet

**Learning Transferable Architectures for Scalable Image Recognition**
Barret Zoph, Vijay Vasudevan, Jonathon Shlens, Quoc V. Le

* code: [keras-applications : https://github.com/keras-team/keras-applications/blob/master/keras\_applications/nasnet.py](https://github.com/keras-team/keras-applications/blob/master/keras_applications/nasnet.py) ⚠️ Archived
* code: [unofficial-keras : https://github.com/titu1994/Keras-NASNet](https://github.com/titu1994/Keras-NASNet) ⭐ 196 | 🐛 9 | 🌐 Python | 📅 2018-05-17
* code: [unofficial-tensorflow : https://github.com/yeephycho/nasnet-tensorflow](https://github.com/yeephycho/nasnet-tensorflow) ⭐ 135 | 🐛 6 | 🌐 Python | 📅 2021-07-08
* code: [unofficial-pytorch : https://github.com/wandering007/nasnet-pytorch](https://github.com/wandering007/nasnet-pytorch) ⭐ 75 | 🐛 2 | 🌐 Python | 📅 2020-12-05
* pdf: <https://arxiv.org/abs/1707.07012>

### MobileNetV2

**MobileNetV2: Inverted Residuals and Linear Bottlenecks**
Mark Sandler, Andrew Howard, Menglong Zhu, Andrey Zhmoginov, Liang-Chieh Chen

* code: [unofficial-keras : https://github.com/xiaochus/MobileNetV2](https://github.com/xiaochus/MobileNetV2) ⭐ 340 | 🐛 15 | 🌐 Python | 📅 2019-05-25
* code: [unofficial-pytorch : https://github.com/Randl/MobileNetV2-pytorch](https://github.com/Randl/MobileNetV2-pytorch) ⭐ 281 | 🐛 6 | 🌐 Python | 📅 2018-08-28
* code: [unofficial-tensorflow : https://github.com/neuleaf/MobileNetV2](https://github.com/neuleaf/MobileNetV2) ⭐ 150 | 🐛 3 | 🌐 Python | 📅 2019-05-07
* pdf: <https://arxiv.org/abs/1801.04381>

### IGCV2

**IGCV2: Interleaved Structured Sparse Convolutional Neural Networks**
Guotian Xie, Jingdong Wang, Ting Zhang, Jianhuang Lai, Richang Hong, Guo-Jun Qi

* pdf: <https://arxiv.org/abs/1804.06202>

### hier

**Hierarchical Representations for Efficient Architecture Search**
Hanxiao Liu, Karen Simonyan, Oriol Vinyals, Chrisantha Fernando, Koray Kavukcuoglu

* pdf: <https://arxiv.org/abs/1711.00436>

### PNasNet

**Progressive Neural Architecture Search**
Chenxi Liu, Barret Zoph, Maxim Neumann, Jonathon Shlens, Wei Hua, Li-Jia Li, Li Fei-Fei, Alan Yuille, Jonathan Huang, Kevin Murphy

* code: [tensorflow-slim : https://github.com/tensorflow/models/blob/master/research/slim/nets/nasnet/pnasnet.py](https://github.com/tensorflow/models/blob/master/research/slim/nets/nasnet/pnasnet.py) ⭐ 77,661 | 🐛 1,273 | 🌐 Python | 📅 2026-09-03
* code: [unofficial-pytorch : https://github.com/chenxi116/PNASNet.pytorch](https://github.com/chenxi116/PNASNet.pytorch) ⭐ 321 | 🐛 3 | 🌐 Python | 📅 2022-08-04
* code: [unofficial-tensorflow : https://github.com/chenxi116/PNASNet.TF](https://github.com/chenxi116/PNASNet.TF) ⭐ 101 | 🐛 3 | 🌐 Python | 📅 2018-12-08
* pdf: <https://arxiv.org/abs/1712.00559>

### AmoebaNet

**Regularized Evolution for Image Classifier Architecture Search**
Esteban Real, Alok Aggarwal, Yanping Huang, Quoc V Le

* code: [tensorflow-tpu : https://github.com/tensorflow/tpu/tree/master/models/official/amoeba\_net](https://github.com/tensorflow/tpu/tree/master/models/official/amoeba_net) ⭐ 5,277 | 🐛 319 | 🌐 Jupyter Notebook | 📅 2026-06-22
* pdf: <https://arxiv.org/abs/1802.01548>

### SENet

**Squeeze-and-Excitation Networks**
Jie Hu, Li Shen, Samuel Albanie, Gang Sun, Enhua Wu

* code: [official : https://github.com/hujie-frank/SENet](https://github.com/hujie-frank/SENet) ⭐ 3,647 | 🐛 16 | 🌐 Cuda | 📅 2019-02-25
* code: [unofficial-pytorch : https://github.com/moskomule/senet.pytorch](https://github.com/moskomule/senet.pytorch) ⭐ 2,343 | 🐛 0 | 🌐 Python | 📅 2021-03-02
* code: [unofficial-tensorflow : https://github.com/taki0112/SENet-Tensorflow](https://github.com/taki0112/SENet-Tensorflow) ⭐ 755 | 🐛 15 | 🌐 Python | 📅 2018-08-14
* code: [unofficial-caffe : https://github.com/shicai/SENet-Caffe](https://github.com/shicai/SENet-Caffe) ⭐ 170 | 🐛 9 | 📅 2018-11-26
* code: [unofficial-mxnet : https://github.com/bruinxiong/SENet.mxnet](https://github.com/bruinxiong/SENet.mxnet) ⭐ 156 | 🐛 6 | 🌐 Python | 📅 2018-07-27
* pdf: <https://arxiv.org/abs/1709.01507>

### ShuffleNetV2

**ShuffleNet V2: Practical Guidelines for Efficient CNN Architecture Design**
Ningning Ma, Xiangyu Zhang, Hai-Tao Zheng, Jian Sun

* code: [unofficial-pytorch : https://github.com/Randl/ShuffleNetV2-pytorch](https://github.com/Randl/ShuffleNetV2-pytorch) ⭐ 198 | 🐛 5 | 🌐 Python | 📅 2022-04-17
* code: [unofficial-keras : https://github.com/opconty/keras-shufflenetV2](https://github.com/opconty/keras-shufflenetV2) ⭐ 98 | 🐛 8 | 🌐 Python | 📅 2018-08-14
* code: [unofficial-caff2: https://github.com/wolegechu/ShuffleNetV2.Caffe2](https://github.com/wolegechu/ShuffleNetV2.Caffe2) ⭐ 25 | 🐛 1 | 🌐 Python | 📅 2018-08-06
* pdf: <https://arxiv.org/abs/1807.11164>
* code: [unofficial-pytorch : https://github.com/Bugdragon/ShuffleNet\_v2\_PyTorch](https://github.com/Bugdragon/ShuffleNet_v2_PyTorch)

### CBAM

CBAM: Convolutional Block Attention Module
Sanghyun Woo, Jongchan Park, Joon-Young Lee, In So Kweon

* code: [official-pytorch : https://github.com/Jongchan/attention-module](https://github.com/Jongchan/attention-module) ⭐ 2,231 | 🐛 42 | 🌐 Python | 📅 2023-03-09
* code: [unofficial-pytorch : https://github.com/luuuyi/CBAM.PyTorch](https://github.com/luuuyi/CBAM.PyTorch) ⭐ 1,500 | 🐛 10 | 🌐 Python | 📅 2023-07-12
* code: [unofficial-keras : https://github.com/kobiso/CBAM-keras](https://github.com/kobiso/CBAM-keras) ⭐ 367 | 🐛 10 | 🌐 Python | 📅 2021-02-08
* code: [unofficial-pytorch : https://github.com/elbuco1/CBAM](https://github.com/elbuco1/CBAM) ⭐ 132 | 🐛 2 | 🌐 Python | 📅 2019-10-18
* pdf: <https://arxiv.org/abs/1807.06521>

### IGCV3

**IGCV3: Interleaved Low-Rank Group Convolutions for Efficient Deep Neural Networks**
Ke Sun, Mingjie Li, Dong Liu, Jingdong Wang

* code: [official : https://github.com/homles11/IGCV3](https://github.com/homles11/IGCV3) ⭐ 189 | 🐛 3 | 🌐 Python | 📅 2018-10-22
* code: [unofficial-pytorch : https://github.com/xxradon/IGCV3-pytorch](https://github.com/xxradon/IGCV3-pytorch) ⭐ 19 | 🐛 4 | 🌐 Python | 📅 2018-06-21
* code: [unofficial-tensorflow : https://github.com/ZHANG-SHI-CHANG/IGCV3](https://github.com/ZHANG-SHI-CHANG/IGCV3) ⭐ 2 | 🐛 1 | 🌐 Python | 📅 2018-06-14
* pdf: <https://arxiv.org/abs/1806.00178>

### BAM

**BAM: Bottleneck Attention Module**
Jongchan Park, Sanghyun Woo, Joon-Young Lee, In So Kweon

* code: [official-pytorch : https://github.com/Jongchan/attention-module](https://github.com/Jongchan/attention-module) ⭐ 2,231 | 🐛 42 | 🌐 Python | 📅 2023-03-09
* code: [unofficial-tensorflow : https://github.com/huyz1117/BAM](https://github.com/huyz1117/BAM) ⭐ 12 | 🐛 1 | 🌐 Python | 📅 2019-01-16
* pdf: <https://arxiv.org/abs/1807.06514>

### MNasNet

**MnasNet: Platform-Aware Neural Architecture Search for Mobile**
Mingxing Tan, Bo Chen, Ruoming Pang, Vijay Vasudevan, Quoc V. Le

* code: [unofficial-pytorch : https://github.com/AnjieZheng/MnasNet-PyTorch](https://github.com/AnjieZheng/MnasNet-PyTorch) ⭐ 275 | 🐛 4 | 🌐 Python | 📅 2018-08-15
* code: [unofficial-keras : https://github.com/Shathe/MNasNet-Keras-Tensorflow](https://github.com/Shathe/MNasNet-Keras-Tensorflow) ⭐ 98 | 🐛 1 | 🌐 Python | 📅 2020-03-05
* code: [unofficial-MxNet : https://github.com/chinakook/Mnasnet.MXNet](https://github.com/chinakook/Mnasnet.MXNet) ⭐ 60 | 🐛 1 | 🌐 Python | 📅 2018-12-27
* code: [unofficial-caffe : https://github.com/LiJianfei06/MnasNet-caffe](https://github.com/LiJianfei06/MnasNet-caffe) ⭐ 52 | 🐛 5 | 🌐 Python | 📅 2018-10-19
* pdf: <https://arxiv.org/abs/1807.11626>

### SKNet

**Selective Kernel Networks**
Xiang Li, Wenhai Wang, Xiaolin Hu, Jian Yang

* pdf: <https://arxiv.org/abs/1903.06586>
* code: [official : https://github.com/implus/SKNet](https://github.com/implus/SKNet)

### DARTS

**DARTS: Differentiable Architecture Search**
Hanxiao Liu, Karen Simonyan, Yiming Yang

* code: [official : https://github.com/quark0/darts](https://github.com/quark0/darts) ⭐ 3,996 | 🐛 95 | 🌐 Python | 📅 2021-01-03
* code: [unofficial-pytorch : https://github.com/khanrc/pt.darts](https://github.com/khanrc/pt.darts) ⭐ 451 | 🐛 33 | 🌐 Python | 📅 2022-07-19
* code: [unofficial-tensorflow : https://github.com/NeroLoh/darts-tensorflow](https://github.com/NeroLoh/darts-tensorflow) ⭐ 72 | 🐛 4 | 🌐 Python | 📅 2018-12-29
* pdf: <https://arxiv.org/abs/1806.09055>

### ProxylessNAS

**ProxylessNAS: Direct Neural Architecture Search on Target Task and Hardware**
Han Cai, Ligeng Zhu, Song Han

* code: [official : https://github.com/mit-han-lab/ProxylessNAS](https://github.com/mit-han-lab/ProxylessNAS) ⭐ 1,448 | 🐛 2 | 🌐 C++ | 📅 2024-08-30
* pdf: <https://arxiv.org/abs/1812.00332>

### MobileNetV3

**Searching for MobileNetV3**
Andrew Howard, Mark Sandler, Grace Chu, Liang-Chieh Chen, Bo Chen, Mingxing Tan, Weijun Wang, Yukun Zhu, Ruoming Pang, Vijay Vasudevan, Quoc V. Le, Hartwig Adam

* code: [unofficial-pytorch : https://github.com/xiaolai-sqlai/mobilenetv3](https://github.com/xiaolai-sqlai/mobilenetv3) ⭐ 1,864 | 🐛 46 | 🌐 Python | 📅 2023-04-27
* code: [unofficial-pytorch : https://github.com/kuan-wang/pytorch-mobilenet-v3](https://github.com/kuan-wang/pytorch-mobilenet-v3) ⭐ 807 | 🐛 9 | 🌐 Python | 📅 2019-06-23
* code: [unofficial-pytorch : https://github.com/d-li14/mobilenetv3.pytorch](https://github.com/d-li14/mobilenetv3.pytorch) ⭐ 597 | 🐛 12 | 🌐 Python | 📅 2023-03-08
* code: [unofficial-pytorch : https://github.com/leaderj1001/MobileNetV3-Pytorch](https://github.com/leaderj1001/MobileNetV3-Pytorch) ⭐ 299 | 🐛 7 | 🌐 Python | 📅 2019-07-04
* code: [unofficial-keras : https://github.com/xiaochus/MobileNetV3](https://github.com/xiaochus/MobileNetV3) ⭐ 242 | 🐛 10 | 🌐 Python | 📅 2020-03-23
* code: [unofficial-caffe : https://github.com/jixing0415/caffe-mobilenet-v3](https://github.com/jixing0415/caffe-mobilenet-v3) ⭐ 131 | 🐛 6 | 📅 2019-05-18
* pdf: <https://arxiv.org/abs/1905.02244>

### Res2Net

**Res2Net: A New Multi-scale Backbone Architecture**
Shang-Hua Gao, Ming-Ming Cheng, Kai Zhao, Xin-Yu Zhang, Ming-Hsuan Yang, Philip Torr

* code: [unofficial-pytorch : https://github.com/4uiiurz1/pytorch-res2net](https://github.com/4uiiurz1/pytorch-res2net) ⭐ 113 | 🐛 5 | 🌐 Python | 📅 2019-04-28
* code: [unofficial-keras : https://github.com/fupiao1998/res2net-keras](https://github.com/fupiao1998/res2net-keras) ⭐ 16 | 🐛 1 | 🌐 Python | 📅 2019-04-07
* pdf: <https://arxiv.org/abs/1904.01169>
* code: [official-pytorch : https://github.com/Res2Net](https://github.com/Res2Net)

### LIP-ResNet

**LIP: Local Importance-based Pooling**
Ziteng Gao, Limin Wang, Gangshan Wu

* code: [official-pytorch : https://github.com/sebgao/LIP](https://github.com/sebgao/LIP) ⭐ 225 | 🐛 0 | 🌐 Python | 📅 2021-09-29
* pdf: <https://arxiv.org/abs/1908.04156>

### EfficientNet

**EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks**
Mingxing Tan, Quoc V. Le

* code: [unofficial-pytorch : https://github.com/lukemelas/EfficientNet-PyTorch](https://github.com/lukemelas/EfficientNet-PyTorch) ⭐ 8,220 | 🐛 167 | 🌐 Python | 📅 2022-04-08
* code: [official-tensorflow : https://github.com/tensorflow/tpu/tree/master/models/official/efficientnet](https://github.com/tensorflow/tpu/tree/master/models/official/efficientnet) ⭐ 5,277 | 🐛 319 | 🌐 Jupyter Notebook | 📅 2026-06-22
* pdf: <https://arxiv.org/abs/1905.11946>

### FixResNeXt

**Fixing the train-test resolution discrepancy**
Hugo Touvron, Andrea Vedaldi, Matthijs Douze, Hervé Jégou

* code: [official-pytorch : https://github.com/facebookresearch/FixRes](https://github.com/facebookresearch/FixRes) ⚠️ Archived
* pdf: <https://arxiv.org/abs/1906.06423>

### BiT

**Big Transfer (BiT): General Visual Representation Learning**
Alexander Kolesnikov, Lucas Beyer, Xiaohua Zhai, Joan Puigcerver, Jessica Yung, Sylvain Gelly, Neil Houlsby

* code: [official-tensorflow: https://github.com/google-research/big\_transfer](https://github.com/google-research/big_transfer) ⚠️ Archived
* pdf: <https://arxiv.org/abs/1912.11370>

### PSConv + ResNext101

**PSConv: Squeezing Feature Pyramid into One Compact Poly-Scale Convolutional Layer**
Duo Li1, Anbang Yao2B, and Qifeng Chen1B

* code: <https://github.com/d-li14/PSConv> ⭐ 174 | 🐛 4 | 🌐 Python | 📅 2020-07-14
* pdf: <https://arxiv.org/abs/2007.06191>

### NoisyStudent

**Self-training with Noisy Student improves ImageNet classification**
Qizhe Xie, Minh-Thang Luong, Eduard Hovy, Quoc V. Le

* code: [official-tensorflow: https://github.com/google-research/noisystudent](https://github.com/google-research/noisystudent) ⚠️ Archived
* pdf: <https://arxiv.org/abs/1911.04252>
* code: [unofficial-pytorch: https://github.com/sally20921/NoisyStudent](https://github.com/sally20921/NoisyStudent)

### RegNet

**Designing Network Design Spaces**
Ilija Radosavovic, Raj Prateek Kosaraju, Ross Girshick, Kaiming He, Piotr Dollár

* code: [official-pytorch: https://github.com/facebookresearch/pycls](https://github.com/facebookresearch/pycls) ⚠️ Archived
* code: [unofficial-pytorch: https://github.com/d-li14/regnet.pytorch](https://github.com/d-li14/regnet.pytorch) ⭐ 69 | 🐛 1 | 🌐 Python | 📅 2021-03-19
* pdf: <https://arxiv.org/abs/2003.13678>

### GhostNet

**GhostNet: More Features from Cheap Operations**
Kai Han, Yunhe Wang, Qi Tian, Jianyuan Guo, Chunjing Xu, Chang Xu

* code: [official-pytorch: https://github.com/huawei-noah/ghostnet](https://github.com/huawei-noah/ghostnet) ⭐ 4,419 | 🐛 94 | 🌐 Python | 📅 2025-03-15
* pdf: <https://arxiv.org/abs/1911.11907>

### ViT

**An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale**
Alexey Dosovitskiy, Lucas Beyer, Alexander Kolesnikov, Dirk Weissenborn, Xiaohua Zhai, Thomas Unterthiner, Mostafa Dehghani, Matthias Minderer, Georg Heigold, Sylvain Gelly, Jakob Uszkoreit, Neil Houlsby

* code: [official-tensorflow: https://github.com/google-research/vision\_transformer](https://github.com/google-research/vision_transformer) ⭐ 12,700 | 🐛 139 | 🌐 Jupyter Notebook | 📅 2026-08-01
* code: [unofficial-pytorch: https://github.com/jeonsworld/ViT-pytorch](https://github.com/jeonsworld/ViT-pytorch) ⭐ 2,163 | 🐛 29 | 🌐 Jupyter Notebook | 📅 2022-06-07
* pdf: <https://arxiv.org/abs/2010.11929>

### DeiT

**Training data-efficient image transformers & distillation through attention**
Hugo Touvron, Matthieu Cord, Matthijs Douze, Francisco Massa, Alexandre Sablayrolles, Hervé Jégou

* code: [official-pytorch: https://github.com/facebookresearch/deit](https://github.com/facebookresearch/deit) ⚠️ Archived
* pdf: <https://arxiv.org/abs/2012.12877>

### PVT

**Pyramid Vision Transformer: A Versatile Backbone for Dense Prediction without Convolutions**
Wenhai Wang, Enze Xie, Xiang Li, Deng-Ping Fan, Kaitao Song, Ding Liang, Tong Lu, Ping Luo, Ling Shao

* code: [official-pytorch: https://github.com/whai362/PVT](https://github.com/whai362/PVT) ⭐ 1,901 | 🐛 41 | 🌐 Python | 📅 2022-10-27
* pdf: <https://arxiv.org/abs/2102.12122>

### T2T

**Tokens-to-Token ViT: Training Vision Transformers from Scratch on ImageNet**
Li Yuan, Yunpeng Chen, Tao Wang, Weihao Yu, Yujun Shi, Zihang Jiang, Francis EH Tay, Jiashi Feng, Shuicheng Yan

* code: [official-pytorch: https://github.com/yitu-opensource/T2T-ViT](https://github.com/yitu-opensource/T2T-ViT) ⭐ 1,191 | 🐛 23 | 🌐 Jupyter Notebook | 📅 2023-10-27
* pdf: <https://arxiv.org/abs/2101.11986>

### DeepVit

**DeepViT: Towards Deeper Vision Transformer**
Daquan Zhou, Bingyi Kang, Xiaojie Jin, Linjie Yang, Xiaochen Lian, Zihang Jiang, Qibin Hou, and Jiashi Feng.

* code: [official-pytorch: https://github.com/zhoudaquan/dvit\_repo](https://github.com/zhoudaquan/dvit_repo) ⭐ 141 | 🐛 12 | 🌐 Python | 📅 2021-12-18
* pdf: <https://arxiv.org/abs/2103.11886>

### ViL

**Multi-Scale Vision Longformer: A New Vision Transformer for High-Resolution Image Encoding**
Pengchuan Zhang, Xiyang Dai, Jianwei Yang, Bin Xiao, Lu Yuan, Lei Zhang, Jianfeng Gao

* code: [official-pytorch: https://github.com/microsoft/vision-longformer](https://github.com/microsoft/vision-longformer) ⭐ 249 | 🐛 8 | 🌐 Python | 📅 2022-03-16
* pdf: <https://arxiv.org/abs/2103.15358>

### TNT

**Transformer in Transformer**
Kai Han, An Xiao, Enhua Wu, Jianyuan Guo, Chunjing Xu, Yunhe Wang

* code: <https://github.com/huawei-noah/CV-Backbones> ⭐ 4,419 | 🐛 94 | 🌐 Python | 📅 2025-03-15
* pdf: <https://arxiv.org/abs/2103.00112>

### CvT

**CvT: Introducing Convolutions to Vision Transformers**
Haiping Wu, Bin Xiao, Noel Codella, Mengchen Liu, Xiyang Dai, Lu Yuan, Lei Zhang

* code: <https://github.com/microsoft/CvT> ⭐ 606 | 🐛 22 | 🌐 Python | 📅 2023-05-16
* pdf: <https://arxiv.org/abs/2103.15808>

### CViT

**CrossViT: Cross-Attention Multi-Scale Vision Transformer for Image Classification**
Chun-Fu (Richard) Chen, Quanfu Fan, Rameswar Panda

* code: <https://github.com/IBM/CrossViT> ⚠️ Archived
* pdf: <https://arxiv.org/abs/2103.14899>

### Focal-T

**Focal Attention for Long-Range Interactions in Vision Transformers**
Jianwei Yang, Chunyuan Li, Pengchuan Zhang, Xiyang Dai, Bin Xiao, Lu Yuan, Jianfeng Gao

* code: [ https://github.com/microsoft/Focal-Transformer](https://github.com/microsoft/Focal-Transformer) ⭐ 559 | 🐛 18 | 🌐 Python | 📅 2022-03-27
* pdf: <https://arxiv.org/abs/2107.00641>

### Twins

**Twins: Revisiting the Design of Spatial Attention in Vision Transformers**

* pdf: <https://arxiv.org/abs/2104.13840>
* code: <https://git.io/Twins>

### PVTv2

**Wenhai Wang, Enze Xie, Xiang Li, Deng-Ping Fan, Kaitao Song, Ding Liang, Tong Lu, Ping Luo, Ling Shao**

* code: [official-pytorch: https://github.com/whai362/PVT](https://github.com/whai362/PVT) ⭐ 1,901 | 🐛 41 | 🌐 Python | 📅 2022-10-27
* pdf: <https://arxiv.org/abs/2106.13797>

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-09-04._
