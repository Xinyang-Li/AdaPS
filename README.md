# AdaPS: Adaptive optimization for multi-foci generation

Multi-foci generation is a problem of **computer-generated holography**. The  purpose is to calculate a phase pattern on the Fourier plane of the lens to generate desired multi-foci distribution. Because of the nonconvexity (both the forward propagation model and the loss function) of this problem, conventional methods have difficulties in solving it.

Here, we use stochastic gradient descent (SGD) to solve this problem. The state-of-the-art SGD algorithm, **Adam optimizer** is employed to guarantee fast and stable convergence. Our method has been verified both in simulations and several experiments related to multiphoton microscopy.

We name this method adaptive optimization-based phase-searching method (**AdaPS**) and hope that our work can be helpful in the field of optics and imaging. More details please refer to the published paper. [[paper]](https://www.osapublishing.org/oe/home.cfm)

<img src="https://github.com/BBNC-Computational-Imaging/AdaPS/blob/master/schemetic.jpg" width="1000" align="middle">


# Adam optimizer

Adam is short for Adaptive Moment Estimation, an adaptive optimization method that applies adaptive learning rates for each parameter, as well as estimating the lower-order moments to accelerate convergence [[paper]](https://arxiv.org/abs/1412.6980). Adam is most commonly used in the training of deep neural networks, where millions of parameters need to be adjusted. Empirical results demonstrate that Adam works well in practice and compares favorably to other stochastic optimization methods.

# Environment

Our code is organized in a jupyter notebook file and has been tested to be executable in the environment listed as below: 
- ubuntu 16.04 
- python 3.6
- **tensorflow-gpu 1.4.0**
- NVIDIA GPU + CUDA 8.0

Please check your environment before running this notebook. If your environment is not consistent, we suggest you configure the same environment to avoid some annoying errors caused by version incompatibility of the Tensorflow platform.

# Citation

If you use this code please cite the corresponding paper where original methods appeared: 

"*Adaptive optimization for axial multi-foci generation in multiphoton microscopy*". [[paper]](https://www.osapublishing.org/oe/home.cfm)
