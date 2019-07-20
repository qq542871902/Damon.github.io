如何处理不同尺寸大小的图片在CNN中训练？
answer:不关心压缩图像，网络可能会学会理解内容;无论如何，缩放和透视对内容意味着什么？
       将图像中心裁剪为特定大小，如果您担心丢失数据，请进行多种裁剪并使用这些裁剪来增加输入数据，以便将原始图像分成N个不同的正确大小的图像
       将图像用纯色填充到平方大小，然后调整大小。
       做一个这样的组合
       Depending on how far you want or need to go, there actually is a paper here called Spatial Pyramid Pooling in Deep Convolution Networks for Visual Recognition that handles inputs of arbitrary sizes by processing them in a very special way.
做修改
