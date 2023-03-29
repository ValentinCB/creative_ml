<div align="center">
<h1>
  <br>
  <a href="http://acids.ircam.fr"><img src="images/logo_acids.png" alt="ACIDS" width="200"></a>
  <br>
  Creative Machine Learning
  <br>
</h1>

<h3>Creative Machine Learning course and notebooks in JAX, PyTorch and Numpy.</h3>

<h4>
  <a href="#lessons">Lessons</a> •
  <a href="#setup">Setup</a> •
  <a href="#administrative">Administrative</a> •
  <a href="#details">Detailed lessons</a> •
  <a href="#contribution">Contribution</a> •
  <a href="#about">About</a>
</h4>
</div>

This repository contains the courses in machine learning applied to music and other creative mediums.
This course is currently given at the University of Tokyo (Japan), and along the [ATIAM Masters](http://atiam.ircam.fr) at IRCAM, Paris (France). 
The courses slides along with a set of interactive Jupyter Notebooks will be updated along the year to provide all the ML program.
This course is proudly provided by the <a href="http://acids.ircam.fr" target="_blank">ACIDS</a> team.
Please first follow the installation procedure (see section) to ensure that you have all necessary libraries to follow the course smoothly. 
You also need to get the audio datasets from this [link ![](../images/file.png)](https://nubo.ircam.fr/index.php/s/oRHRMCYNDXc5cWJ)   

**As the development of this course is always ongoing, please pull this repo regularly to stay updated.**
**Also, please do not hesitate to post issues or PRs if you spot any mistake** (see the [#contribution](contribution section)).

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li> <a href="#lessons">Lessons</a> </li>
    <li>
      <a href="#projects"> ➤ Projects</a>
      <ul>
        <li><a href="#preprocessed-data">Pre-processed data</a></li>
        <li><a href="#statistical-feature">Statistical feature</a></li>
        <li><a href="#topological-feature">Topological feature</a></li>
      </ul>
    </li>
    <li> <a href="#adminiistrative">Datasets</a> </li>
    <li> <a href="#details">Detailed lessons</a> </li>
    <li> <a href="#contribution">Contribution</a> </li>
    <li> <a href="#about">About</a> </li>
  </ol>
</details>


## Lessons

---

### [00 - Introduction](00_introduction.pdf)

[![Slides](https://img.shields.io/badge/Slides-online-7DA416.svg?style=flat-square&logo=googledrive)](https://github.com/acids-ircam/ddsp_pytorch) 
[![Powerpoint](https://img.shields.io/badge/Slides-download-167DA4.svg?style=flat-square&logo=files)](https://github.com/acids-ircam/ddsp_pytorch) 
[![Colab](https://img.shields.io/badge/Notebook-collab-7DA416.svg?style=flat-square&logo=googlecolab)](https://arxiv.org/abs/2001.04643) 
[![Notebook](https://img.shields.io/badge/Notebook-download-167DA4.svg?style=flat-square&logo=jupyter)](https://github.com/acids-ircam/ddsp_pytorch) 
[![Video on YouTube](https://img.shields.io/badge/Video-None-7D1616.svg?style=flat-square&logo=Youtube)]()
[![Published in ArXiV](https://img.shields.io/badge/Paper-None-7D1616.svg?style=flat-square&logo=arXiv)](https://arxiv.org/abs/2001.04643) 

General introduction
Application examples
Course specificities
Install and setup
Pre-requisites
Toolboxes and tutorials
Introducing machine learning

- [01 - Machine learning](01_machine_learning.pdf)
    - [Notebook - Machine learning](01a_machine_learning.ipynb)
    - [Notebook - Feature-based learning](01b_feature_based_learning.ipynb)
Problem statement
Classical problems
Linear models for regression and classification
Optimization and Initialization
Overfitting and cross-validation
Properties and complexity

- [02 - Neural networks](02_neural_networks.pdf)
    - [Notebook - Neural networks](02_neural_networks.ipynb)
Brief history
The artificial neuron
Geometric perspective on neurons
Gradient descent
Multi-layer perceptron
Backpropagation

- [03 - Advanced Neural Networks](03_advanced_networks.pdf)
    - [Notebook - Advanced networks](03_advanced_networks.ipynb)
Convolution
Convolutional NN
Recurrent NN
Regularization

- [04 - Deep learning](04_deep_learning.pdf)
    - [Notebook - Deep learning](04a_deep_learning.ipynb)
    - [Notebook - Auto-encoders](04b_auto_encoders.ipynb)
Residual networks
Attention and transformers
Auto-encoders
Modern applications

- [05 - Probabilities and Bayesian inference](04_probabilities_bayesian.pdf)
    - [Notebook - Probabilities and distributions](05a_probabilities.ipynb)
    - [Notebook - Bayesian inference](05b_bayesian_inference.ipynb)
Rules of probability
Conditional and marginal
Expectation
Notable distributions
Sampling
Bayesian probability
Probabilistic inference
Maximum A Posteriori
Maximum Likelihood
Conjugate distributions
    
- [06 - Latent models](06_latent_expectation_maximization.pdf)
    - [Notebook - Latent clustering and kMeans](06a_latent_models.ipynb)
    - [Notebook - Gaussian Mixture Models](06b_gaussian_mixture_models.ipynb)
Unsupervised learning
Clustering
Latent variables
Expectation-Maximization
Q-Function
Variational derivation
Gaussian Mixtures

- [07 - Approximate inference](07a_approximate_inference.ipynb)
    - [Notebook - Sampling](07b_sampling_mcmc.ipynb)
Sampling
Monte-Carlo and rejection
Metropolis-Hastings
Variational inference
Deriving variational inference
    
- [08 - Variational Auto-Encoder (VAE) and flows](08_variational_ae_flows.pdf)
    - [Notebook - Variational auto-encoders](08a_variational_auto_encoders.ipynb)
    - [Notebook - Normalizing flows](08b_normalizing_flows.ipynb)
Auto-Encoders
Variational Inference
VAEs and properties
beta-VAE and disentanglement
Normalizing flows
Flows in VAEs
    
- [09 - Adversarial learning](09_adversarial_learning.pdf)
    - [Notebook - Generative Adversarial Networks](09a_generative_adversarial_network.ipynb)
Estimating by comparing
Deriving the adversarial objective
Generative Adversarial Networks
Adversarial attacks
Flaws of GANs
Modern applications

- [10 - Diffusion models](10_diffusion_models.pdf)
    - [Notebook - Diffusion models](10a_diffusion_models.ipynb)
Diffusion models
Score-based approach
Langevin dynamics

- [11 - Guest lecture]

## Setup

Along the tutorials, we provide a reference code for each section. 
This code contains helper functions that will alleviate you from the burden of data import and other sideline implementations. 
You will find designated spaces in each file to develop your solutions. 
The code is in Python (notebooks impending) and relies on the concept of [code sections](https://fr.mathworks.com/help/matlab/matlab_prog/run-sections-of-programs.html),
 which allows you to evaluate only part of the code (to avoid running long import tasks multiple times and concentrate on the question at hand.

### Dependencies

#### Python installation

In order to get the baseline script to work, you need to have a working distribution of `Python 3.5` as a minimum (we also recommend to update your version to `Python 3.7`). We will also be using the following libraries

- [Matplotlib](https://matplotlib.org/)
- [Numpy](https://numpy.org/)
- [SciPy](https://www.scipy.org/)
- [Scikit-Learn](https://scikit-learn.org/)
- [Music21](http://web.mit.edu/music21/)
- [Librosa](http://librosa.github.io/librosa/index.html)
- [PyTorch](https://pytorch.org/)

We highly recommend that you install [Pip](https://pypi.python.org/pypi/pip/) or [Anaconda](https://www.anaconda.com/download/) that will manage the automatic installation of those Python libraries (along with their dependencies). If you are using `Pip`, you can use the following commands

```
pip install matplotlib
pip install numpy
pip install scipy
pip install scikit-learn
pip install music21
pip install librosa
pip install torch torchvision
```

For those of you who have never coded in Python, here are a few interesting resources to get started.

- [TutorialPoint](https://www.tutorialspoint.com/python/)
- [Programiz](https://www.programiz.com/python-programming)

#### Jupyter notebooks and lab

In order to ease following the exercises along with the course, we will be relying on [**Jupyter Notebooks**](https://jupyter.org/). If you have never used a notebook before, we recommend that you look at their website to understand the concept. Here we also provide the instructions to install **Jupyter Lab** which is a more integrative version of notebooks. You can install it on your computer as follows (if you use `pip`)

```
pip install jupyterlab
```

Then, once installed, you can go to the folder where you cloned this repository, and type in

```
jupyter lab
```


## Administrative 

These administrative details concerns only the current physical session attached to the corresponding university.

**Type**   : 2-credits graduate school course  \\
**Period** : April - July 2023 \\
**Span**   : 13 classes of 105 minutes \\
**Date**   : Thursday at 2:55 - 4:40 pm (JST Time) \\
**Onsite** : Room 214, 2nd Floor, Sci. 7 Building \\
**Online** : https://u-tokyo-ac-jp.zoom.us/j/81363691008?pwd=cmxiRURMdm9udXBKbTNjQkZvblNFQT09

**Full calendar** \\
_April_  6, 13, 20, 27 \\
_May_    11, 18, 25 (4th is public holiday) \\
_June_   8, 15, 22, 29 (1st is midterm exam date) \\
_July_   6, 13


## Contribution

Please take a look at our [contributing](CONTRIBUTING.md) guidelines if you're interested in helping!

## About

Code and documentation copyright 2012-2023 by all members of ACIDS. Code released under the [CC-BY-NC-SA 4.0 licence](https://creativecommons.org/licenses/by-nc-sa/4.0/).
