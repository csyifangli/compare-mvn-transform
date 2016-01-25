
Comparison of Multivariate Gaussian transformations
---------------------------------------------------

Example code for presenting the comparison of MVN using: sampling, linearization (like EKF) and unscented transformation (like UKF).

The code simplifies the testing for different conditions and provides a 2x3 plot with input in the rows, and outputs in the columns (flattened over 2D).

Metrics for comparing the resulting gaussians are also provided: KL, BC, DB and Frichet. Note that Frichet depends on chol so it is less reliable with semidefinite variances.

Example below of Function: [x2; 2x1(x2+x1)] evaluated at the Gaussian with mean [0.0054,1.01] and covariance [0.1525,-0.0823,",0.0575]. Sampling done with 500 points.

![Example of result for the function [x2; 2x1(x2+x1)] with point [0.0054,1.01] and variance [0.1525,-0.0823;-0.0823,0.0575] with sampling of 500](example.png)

Related:
* Merwe PhD Thesis about UKF
* Lorenzo Peppoloni PhD Thesis where discussing this issue for our motion reconstruction works