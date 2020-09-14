# KNU CT IMAGE

## 1 Sample Data

|MODEL|EPOCH|LR|OPTIM|RMSE|PSNR|SSIM|
|:------:|:---:|:---:|:---:|:---:|:---:|:---:|
|CNN with Simplified SE Blocks|300|0.0001|ADAM|27.1932|39.1799|**0.9888**|
|6Convolution layers|300|0.0001|ADAM|27.1812|39.2403|0.9875|
|Nested UNet|300|0.001|ADAM|26.4105|39.4375|0.9842|
|ANUNet|300|0.001|ADAM|**22.0937**|**39.9585**|0.9880|

## 5 Sample Data

|MODEL|EPOCH|LR|OPTIM|RMSE|PSNR|SSIM|
|:------:|:---:|:---:|:---:|:---:|:---:|:---:|
|6Convolution layers|300|0.001|ADAM|11.2350|45.8378|0.9883|
|12 SE Blocks|300|??|ADAM|??|??|??|
|12 SE RCAB|300|??|ADAM|??|??|??|
|12 SE DRLM|300|??|ADAM|??|??|??|
|ANUNet|300|??|ADAM|??|??|??|

# 9.14 Update
기존 dcm -> tif -> numpy -> tensor을 dcm -> numpy -> tensor로 변경

5 Data sample 4 for trainval(8:2) 1 for test

12 (Densely) Residual Channel Attention Block Implementation.

# TODO

- [ ] 12 (Densely) Residual Channel Attention Block Network Train/Test

- [ ] Input Image Skip Connection -> good? bad?

- [ ] Residual Net, Densly Residual Net Comparison

# Convolutional Neural Net with Simplified Squeeze-and-Excitation Blocks

Eun, D., Woo, I., Park, B., Kim, N., Lee A, S. M., & Seo, J. B. (2020). "CT kernel conversions using convolutional neural net for super-resolution with simplified squeeze-and-excitation blocks and progressive learning among smooth and sharp kernels." Computer Methods and Programs in Biomedicine

[[Link]](https://www.sciencedirect.com/science/article/abs/pii/S0169260720314486)

## Overview

![Alt text](/Figs/SE.jpg)
 
 Figure 1.Convolutional neural net for super-resolution with simplified squeeze-and-excitation blocks

# CNN architecture consists of six convolutional layer

Lee, S. M., Lee, J.-G., Lee, G., Choe, J., Do, K.-H., Kim, N., & Seo, J. B. (2019). "CT Image Conversion among Different Reconstruction Kernels without a Sinogram by Using a Convolutional Neural Network". Korean Journal of Radiology

[[Link]](https://pc.kjronline.org/DOIx.php?id=10.3348/kjr.2018.0249)

## Overview

![Alt text](/Figs/6Conv.jpg)
 
 Figure 1. Overview of CNN architecture consists of six convolutional layers

# U-Net: Convolutional Networks for Biomedical Image Segmentation

Ronneberger, O., Fischer, P., & Brox, T. (2015). "U-Net: Convolutional Networks for Biomedical Image Segmentation." Medical Image Computing and Computer-Assisted Intervention – MICCAI 2015

[[Link]](https://arxiv.org/pdf/1505.04597v1.pdf)

## Overview

![Alt text](/Figs/Unet.JPG)
 
 Figure 1. Overview of UNet

# UNet++: A Nested U-Net Architecture for Medical Image Segmentation

Zhou, Z., Rahman Siddiquee, M. M., Tajbakhsh, N., & Liang, J. (2018). "UNet++: A Nested U-Net Architecture for Medical Image Segmentation." Lecture Notes in Computer Science

[[Link]](https://arxiv.org/pdf/1807.10165.pdf)

## Overview

![Alt text](/Figs/Unet++.JPG)
 
 Figure 1. Overview of Unet++

# Image Super-Resolution Using Very Deep Residual Channel Attention Networks

Yulun Zhang, Kunpeng Li, Kai Li, Lichen Wang, Bineng Zhong, and Yun Fu, "Image Super-Resolution Using Very Deep Residual Channel Attention Networks", ECCV 2018,

[[Link]](https://arxiv.org/pdf/1807.02758.pdf)

## Overview

![Alt text](/Figs/CA.png)
 
 Figure 1. Overview of ChannelAttention

![Alt text](/Figs/RCAB.png)
 
 Figure 2. Overview of RCAB

![Alt text](/Figs/RCAN.png)
 
 Figure 3. Overview of RCAN

 # Densely Residual Laplacian Super-Resolution

Saeed Anwar, [Nick Barnes], "Densely Residual Laplacian Super-resolution", IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI), 2020.

[[Link]](https://arxiv.org/pdf/1906.12021v2.pdf)

## Overview

![Alt text](/Figs/LaAttention.JPG)
 
 Figure 1. Overview of Laplacian attention

![Alt text](/Figs/DRLM.JPG)
 
 Figure 2. Overview of DRLM

