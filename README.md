# CornerNet_Lite
learn note of CornerNet_Lite

paper-[**CornerNet-Lite: Efficient Keypoint Based Object Detection**](https://arxiv.org/abs/1904.08900)  
Hei Law, Yun Teng, Olga Russakovsky, Jia Deng  
*arXiv:1904.08900* 

project-[**princeton-vl/CornerNet_Lite**](https://github.com/princeton-vl)

# model architecture

CornerNet_Saccade

![arch](https://github.com/tc-qaq/CornerNet_Lite/blob/master/saccade.png)

CornerNet_Squeeze

![arch](https://github.com/tc-qaq/CornerNet_Lite/blob/master/squeeze.jpg)

# Modules

corner_pool

![corner_pool](https://github.com/tc-qaq/CornerNet_Lite/blob/master/corner_pool.png)

pre_mod

![pre_mod](https://github.com/tc-qaq/CornerNet_Lite/blob/master/pre_mod.png)

_decode

![decode](https://github.com/tc-qaq/CornerNet_Lite/blob/master/decode.png)

# hg-featurmap-channels

64-32-16-8-4-8-16-32-64

256-256-384-384-512-384-384-256-256
