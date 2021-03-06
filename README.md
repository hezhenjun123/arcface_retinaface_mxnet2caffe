# arcface_retinaface_mxnet2caffe
arcface and retinaface model convert mxnet to caffe.  
Merge BN and Scale into Conv/FC.

# Operator Support Lists
Convolution  
ChannelwiseConvolution  
BatchNorm  
Activation  
ElementWiseSum  
_Plus  
Concat  
Crop  
Pooling  
Flatten  
FullyConnected  
SoftmaxOutput&SoftmaxFocalOutput  
SoftmaxActivation  
LeakyReLU  
elemwise_add  
UpSampling  
Deconvolution  
Clip  
Reshape  
SoftmaxActivation  
Dropout  
softmax  

# Tested models
[arcface/mobilefacenet-res2-6-10-2-dim512](https://pan.baidu.com/s/1_0O3kJ5dMmD-HdRwNR0Hpw#list/path=%2F) from ZQCNN  
[arcface/model-r34-amf-slim](https://github.com/deepinsight/insightface/wiki/Model-Zoo)  
[retinaface/mnet.25](https://github.com/deepinsight/insightface/issues/669)  
[retinaface/R50](https://pan.baidu.com/s/1C6nKq122gJxRhb37vK0_LQ)  

# Merge BN and Scale into Conv/FC
[Caffe模型合并BN和Scale到Conv/FC层](Caffe模型合并BN和Scale到Conv/FC层)  

# Bugs
R50 Maxpool, caffe use ceil to compute the output shape. Mxnet can use ceil and floor.  

# Reference
[advanced-mxnet2caffe](https://github.com/szad670401/advanced-mxnet2caffe)  
