# Score-based_generative_model

### Summary
This repository contains score-based diffusion models for basic image denoising and Bayesian inverse problems. 

### Description
The score-based diffusion models were inspired by Yang Song's score-based diffusion model and the models are modified versions of them.

#### Model Architecture:
The score-based models use **U-net architecture**, which is a deep neural network architecture designed for image segmentation. U-net is efficient in terms of learning and manages to learn difficult problems with small amount of data.

#### Model Framework:
The model uses **Pytorch** as its deeplearning framework, because it is flexible and highly optimized for GPUs.

#### Stochastic Differential Equation (SDE):
The score-based models use forward and reverse **Ornstein-Uhlenbeck processes** as SDEs in the model, because the forward process can be solved explicitly and the processes are also simple in form, which makes them easy to control.

#### Requirements
- NVIDIA GPU (Recommended)
- Libraries in requirements.txt file installed

#### Additional links:
More information about score-based diffusion models can be found from these links below:

- [Score-based diffusion modelling for image denoising](https://arxiv.org/pdf/2011.13456)
- [Score-based diffusion models in inverse problems](https://arxiv.org/pdf/2111.08005)
- [Conditioal score-based diffusion models using Ornstein-Uhlenbeck processes](https://arxiv.org/pdf/2305.19147)

#### File Descriptions:
- In USDM.ipynb file is a setup for *Unconditional Score-based Diffusion Model* to solve image denoising problems
- In CSDM.ipynb file is a setup for *Conditional Score-based Diffusion Model* Score-based diffusion model to solve Bayesian inverse problems in medical imaging
- ckpt.pth contains a saved model
- MNIST folder contains the dataset
- Requirements.txt contains the list of libraries for the setup






