# 特点
real-time pixelwised semantic segmentation
# 网络结构
## encoder network
1. 13 convolutional layers correspond to the first 13 convolutional layers in the VGG16 network
2. Each encoder in the encoder network performs convolution with a filter bank to produce a set of feature maps
3. Then **batch normalized**
4. ReLU
5. max-pooling with a 2 x 2 window and stride 2
6. save **boundary information**: memorize the max position
7. 

## decoder network
1. 13 layers corresponding the encode network
2. 
## pixelwise classification layer
