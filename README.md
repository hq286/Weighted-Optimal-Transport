# Weighted-Optimal-Transport
This is the code for my master thesis project on optimal transport between images. Special thanks to Dr. Esteban Tabak, Dr. Debra Laefer and Dr. Monty Essid
## Progress 
The main code computes the linear map that minimizes KL-Divergence of two sets of samples with weights (i.e. two pixel images, weights being their pixel intensities). The algorithm that includes nonlinear terms in the optimal map is still under construction and testing.
## Main files
* OT.ipynb is a new version of Dr.Monty Essid's work on Adaptive Optimal Transport on 2D sampels with no weights. This verson has slight changes in the minimax solver which uses Hessian approximation and also includes a another minimax solver which uses Quasi-Newton method and avoids the computation and inverson of Hessian matrix.
* wot_linear.ipynb is the code that compute the optimal linear map that pair two sets of weighted samples, i.e. two pixel images with pixels intensities. As the map is linear in 2D space, it captures changes of images in displacement, scalings and rotations.
* Experiments_on_linear_maps.ipynb is a documents that describes the setting and sythetic examples in more details. It also has some plots of experiment results on those synthetic examples and convergence rate of the algorithm
