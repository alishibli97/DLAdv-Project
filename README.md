# DD2412 Deep Learning, Advanced Course, Project


In this project, we present our re-implementation of the paper [Getting a CLUE](https://arxiv.org/abs/2006.06848) on uncertainty estimations in tensorflow.

For BNN and VAE training, and CLUE generation for COMPAS and LSAT, notebooks ready to run on Colab, our code and pre-trained weights can be found on [drive](https://drive.google.com/drive/folders/1-9qUsgcklq2Mrx_ScDG134BViOOUO8nI?usp=sharing).

You can find the report at [Reproducible CLUEs:A Basic Framework-Invariance Test](https://drive.google.com/file/d/1JwwInzpZ5ZHuW91SV6CLGeZNSRsKIIQ2/view?usp=sharing).

# Abstract
In this project we aimed to replicate the central method of the paper "Getting a CLUE: A Method for Explaining Uncertainty Estimates" and essential components used in their more thorough experiments. We approach reproducibility from a deep learning framework perspective, attempting to reproduce the original PyTorch implementation in TensorFlow. Explainability solutions that are unable to extend to different frameworks are fundamentally at odds with the goals of this task. Thus, we believe that although our results are based on structures that very closely follow the original ones, instead of parting from the method at the top-level, they are an important lower bound to test the framework-invariance of the method, in other words: if a module-by-module translation (or something close to it) into another framework cannot achieve congruent results, what could we expect when increasing implementation flexibility?

We succeeded in the training and implementation of the main components for this method, and most importantly in generating "CLUEs" with our implementation for two selected datasets used in the original paper. We concluded that our FrameWork-Invariance test supports the reproducibility of the method across frameworks, and point to relevant next directions to elaborate on our results. Regardless, we were still had a few complications in terms of reproducibility with the current documentation, which we discuss in detail.

# Structure
The tensorflow implemenetation of the architectures are presents in the following folders:

[BNN: Bayesian Neural Network](https://github.com/alishibli97/DLAdv-Project/tree/main/BNN) 

[VAE: Variational Autoencoder](https://github.com/alishibli97/DLAdv-Project/tree/main/VAE) 

[CLUE ](https://github.com/alishibli97/DLAdv-Project/tree/main/CLUE) 

[VAEAC: Variational Auto-encoding Auto Conditioning](https://github.com/alishibli97/DLAdv-Project/tree/main/VAEAC)

# Source Control

Python 3.8

Tensorflow 2.6.1

Torch 1.10.0

# Citation

Javier Antorán, Umang Bhatt, Tameem Adel, Adrian Weller & José Miguel Hernández-Lobato (2021). Getting a CLUE: A Method for Explaining Uncertainty Estimates.
