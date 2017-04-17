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

## decoder network
1. upsamples its input feature map(s) using the memorized max-pooling indices -> produces
sparse feature map
2. convolved with a trainable decoder filter bank to produce dense feature maps
3. softmax
## pixelwise classification layer
