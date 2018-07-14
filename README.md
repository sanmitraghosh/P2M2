# Probabilistic Programming for inference in Mechanistic Models using PyMC3 and Edward
These are examples that showcase the power of probabilistic programs for model and parameter inference in mechanistic models described as non-linear ODE. This gives us the unique abitlty to solve inverse problems involving mechanistic models written in any language (as long as that model can be wrapped in python) using a ppl such as PyMC3. This essentially frees the modeller from the task of wrting, debugging and testing bespoke inference algorithms.

At the present examples are written in PyMC3. However, I am going to add examples in Edward and other ppls soon.
## Schematic: Inverse problems in biology
![schematic of Inverse problems](https://github.com/sanmitraghosh/P2M2/blob/master/UQ_Picture.png)
## Background

Familiarity with MCMC, sensititivity analysis, inverse problems and autodifferentiation (or knowledge of Backpropagation algorithm) would be useful.
## Installation
To install PyMC3 read the following:
http://docs.pymc.io/notebooks/getting_started.html#Installation
## Usage
All these examples are written in a tutorial fashion and thus I strongly recommend to follow the tutorial ordering.
Materials covered are as follows:

1) Tutorial 1: Example that shows how to wrap a model using Theano `as_op` and use the SMC algorithm. [click here to interact live with these examples](https://mybinder.org/v2/gh/sanmitraghosh/P2M2/master)
2) Tutorial 2 & 3: Examples that show how to write a custom differentiable op in Theano to define a custom ODE layer. NB: Go through these ones carefully as I would use similar techniques to write custom ODE layer using TensorFlow and PyTorch.
3) Tutorial 4: Model selection 
4) Tutorial 5: In this tutorial I will use variational inference, a faster alternative to MCMC, to learn the Fitzhugh-Nagumo model parameters. 
## TODO: 
1) Add Theano Scan RK4 solver.
2) Add Edward (TensorFlow `py_func`) HMC, Gibbs for hierarchical example from disk, and add TensorFlow Probability AIS example.
3) Add Lambdify for sensitivity equation automation.

