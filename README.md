# Deep-Generative-Models
This repository contains my work for the project Deep Generative Models during Summer '2024. In this project we explore various Generative Models for image generation like GANs, VAEs and Diffusion Models.

# Weekly Tasks:
## Week 1: GANs
1. Train a DCGAN on a dataset of your choice and document:
    1. the loss curve (for all types of losses)
    2. the minimum error observed
  
## Week 2: VAEs
We know that a VAE normally consists of an encoder-decoder architecture. The encoder is the part of the model with layers with consecutively lesser no. of neurons (for eg. [200, 100, 50, ..]) and the decoder has layers with increasing number of neurons. The encoder is said to downsample i.e. reduce the dimensionality of the input, turning it into a somewhat condensed form; and the decoder is said to upsample (expand the dimensions).

A. Knowing this, write a VAE:

1. much like the one in the tutorialwith an encoder(left) and decoder(right) - basic vanilla VAE implementation
2. where the encoder (left) is replaced with an encoder-decoder architecture (both downsampling-upsampling)
3. where the decoder (right) is replaced with an encoder-decoder architecture (both downsampling-upsampling)
4. where both sides - encoder and decoder - are replaced with encoder-decoder architecture

B. Compare results of accuracy and output images across all 3 parts of A and comment on which architecture is the best

An encoder-decoder architecture is one where a decoder is attached right after the encoder.
It would have layers with decreasing size, reach a minimum , followed by layers of increasing size.

## Week 3: Diffusion Models
A. Implement a diffusion model.

1. Produce results with 2 sets of hyperparameters - varying learning rate, noising schedule (beta), number of denoising steps.

Attach loss curves for both trainings. Justify your choice of parameters and comment on how your observations vary/agree with what you expected

1. Produce one sample from each class (10 classes) in the CIFAR-10 dataset

B. Instead of starting with complete Gaussian Noise (conventional method), start with a partially noised sample (noisy sample) and denoise it. Do this exercise for a sample that has been noised for:

1. 50 iterations
2. 10 iterations
3. 5 iterations

Comment on the level to which the model is able to denoise your noisy sample and identify any new features/shapes it has added to the image while denoising it.


