+++
authors = ["Xiaotong Li"]
title = "Gradient Enhanced Neural Networks for Optimization of Mars Low Reynold Number Airfoil"
date = "2023-04-20"
description = "Bachelor Research Program"
tags = [
    "UAV",
    "Dynamic transformation",
    "Planning",
]
categories = [
    "Research Project"
]
series = ["Research Project"]
+++


<!--more-->

The project uses improved gradient-enhanced neural network as a surrogate model instead of CFD simulation calculation to predict the aerodynamic parameters of airfoils. By comparing and testing the traditional neural network, the gradient-enhanced neural network(mSANN) and the improved gradient-enhanced neural network, the superiority of the network in terms of prediction performance and convergence speed is clarified. 

<!-- <div align="center"><img height=auto width=auto src=../../images/gradient1.jpg /></div> -->
<div style="text-align:center">
  <img height=auto width=auto src=../../images/gradient1.jpg>
  <center><span style="font-size: 15px;">Figure 1: The accuracy and convergency of different networks</span> </center>
</div>

For the preprocessing of data, this paper uses singular value decomposition to parameterize airfoils and decompose airfoils into modes and modal coefficients. The inverse distance-weighted interpolation method is used to construct a constraint function to limit the modal coefficient and exclude abnormal airfoils. 

<div style="text-align:center">
  <img height=auto width=auto src=../../images/gradient2.jpg>
  <center><span style="font-size: 15px;">Figure 2: The first five airfoil camber and thickness modes obtained by SVD decomposition of UIUC airfoil database</span> </center>
</div>

Latin hypercube sampling was used to generate airfoil samples, and ADflow was used to calculate the aerodynamic parameters and their derivatives. The results are used for the training of the improved gradient-enhanced neural network to obtain a surrogate model for the prediction of the aerodynamics, and the neural network is coupled with the optimization software package for airfoil aerodynamic optimization. Compared with the high-fidelity CFD based optimization method, the optimization results are almost indistinguishable, but the optimization time is greatly reduced.

<div style="text-align:center">
  <img height=auto width=auto src=../../images/gradient3.jpg>
  <center><span style="font-size: 15px;">Figure 3: Grids of airfoils computed by pyHyp</span> </center>
</div>

{{< notice info >}}
Chinese version paper [here](../../uploads/paper.pdf)
{{< /notice >}}