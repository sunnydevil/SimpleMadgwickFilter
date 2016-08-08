# Pitch Angle Estimation of Two Wheel Platform Using EKF and Madgwick Filter
Having a two wheel platform being able to balance requires an accurate estimate of it’s pitch angle, w.r.t. the vertical axis. This project implements the Madgwick and extended Kalman filter algorithm as estimators for this problem using data from an Inertial Measurement Unit. The Madgwick filter uses a quaternion representation of the orientation and a gradient descent method to estimate the angle in a computationally efficient way. The extended Kalman filter exploit the assumption that the noise is gaussian and using Bayes filter to estimate the mean of the state. The performance of the filters are then analysed based on the parameter settings and a final comparison shows that both are almost equally accurate(both static RMS error < 0.2◦) and where the Madgwick filter is 25% faster.
## Installation and Usage
The filters are implemented in [MATLAB](http://se.mathworks.com/products/matlab/).