# Image-Restoration

## Overview 

This project presents a sophisticated deep neural network model designed for image denoising tasks. The model integrates components from the Denoising Convolutional Neural Network (DnCNN) architecture, Convolutional Vision Transformer (CVT), and PixNet. This combination enhances the model's capability to capture both short-range and long-range dependencies in image patches.

## Model Architecture 

<img width="725" alt="1 3" src="https://github.com/Chai-mae/Image-restoration/assets/93831197/55c6488d-dc96-409f-9bb9-856b80a13882">


DnCNN Component:
dncnn: The core architecture of DnCNN, defined as a sequential module comprising multiple convolutional layers with ReLU activation functions and batch normalization layers. This component is dedicated to image denoising tasks.

CVT and PixNet Components:
cvt: An additional module introducing convolutional layers and a Convolutional Vision Transformer (CVT) module. The CVT module comprises two instances of the Transformer module, labeled as 'transformer_0' and 'transformer_1.' Each transformer module includes pre-normalization, attention mechanisms, MLP layers, and post-normalization. The attention component performs self-attention operations on input data, enhancing the model's ability to capture long-range dependencies and relationships between image patches.

embedding: A convolutional layer responsible for transforming input data.

Common Building Blocks:
Conv2d, BatchNorm2d, ReLU: Standard building blocks of convolutional neural networks. Conv2d represents a convolutional layer, BatchNorm2d represents a batch normalization layer, and ReLU represents the rectified linear unit activation function.

## Results

<img width="1034" alt="1 2" src="https://github.com/Chai-mae/Image-restoration/assets/93831197/9d64cf93-2c33-4ca8-8634-1fbd95952e61">

<img width="658" alt="1 1" src="https://github.com/Chai-mae/Image-restoration/assets/93831197/961a8e7e-e383-4505-9d75-56342a899201">
