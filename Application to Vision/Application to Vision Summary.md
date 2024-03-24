# Application of Transformer in Vision: Vision Transformer

Introduced at ‘An Image is Worth 16x16 Words: Transformer for Image Recognition at Scale (Google, 2020)’

After applying Transformer in NLP, researchers wondered if we can apply Transformer in Vision as well.
Here ViT (Vision Transformer) comes in!!
Vit is the first key innovation of Transformer in Vision.

# Vision Transformer Characteristics
- Vit uses self-attention and it treats the whole image at once
  - As we are using self-attention mechanism, we can capture global relationships between different image patches
  - CNN model with convolution layers treats the image in many convolution layers extracting different features in different convolution layers
- ViT doesn’t have a decoder, it only has an encoder
- Input would be image patches and patches go through positional encoding to provide spatial information of the patches and then it is concatenated
  - Image Patches -> Positional Encoding -> Concatenation
- ViT is used to classify an image. For example, through ViT, we can classify an image a bird, car etc.

# Shortcomings of Vision Transformer
- ViT model can not fully reflect the image characteristics of 2D images as the image patch is inputted from image left to right, top to bottom
- ViT model uses a lot of computing force when the image size is large (=when we have huge number of patches)

-> Swin Transformer or CvT model were proposed

Swin Transformer was a big breakthrough in Vision Recognition!

# Swin Transformer
Introduced at ‘Swin Transformer: Hierarchical Vision Transformer using Shifter Windows (Microsoft, 2021)’

Implementing Transformer from text to image, challenges are
- Existence of a different size of entities in an image
- Resolution of image is high compared to a text
-> Swin Transformer is introduced!

## Shifted Windows
- limit self-attention to non-overlapping local windows
- allow cross-window connection

Each time, the attention window is shifted with respect to the previous layers


## What are the differences btw ViT and Swin Transformer?

### ViT
  
Same number and size of patches used for every single layer that goes through the attention mechanism
Can’t get small, large details as much as swin transformer

### Swin Transformer
  
Different number and size of patches used for each of the layers that goes through the attention mechanism
Able to get small, large details much better than ViT!

# Swin Transformer Characteristics
- Hierarchical Architecture
  - Patch number, size are different in each of the hierarchical layers
  - Captures both local and global information
- Shifted Windows
  - Unlike ViT that uses fixed-size patches, Swin makes the receptive field of neighboring patches to overlap
- Local and Global Attention
  - Local attention captures the fine-grained details
  - Global attention captures the characteristics of the entire image
 
# Swin Transformer Architecture
- Image Partitioning
  - Divided into patches
- Linear Embedding
  - Each of the patches becomes a vector
- Swin Transformer Block
  - Multi-head Self-Attention Mechanism
  - Feed-Forward Neural Network(FFNN)
  - Residual Connection
  - Layer Normalization
  - Position-wise Feed-Forward Networks(PFFNs)
- Patch Merging
  - Performs a classification of the entire image










