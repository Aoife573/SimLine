In the example (HD110058_C) we fit CI absorption lines in the edge-on debris disk orbiting HD110058. The data was observed by HST in the UV using the STIS instrument in combination with either the E140H or the E230H grating. The example demonstrates the following steps:

1 - Extracting Relevant Data: Extract the desired absorption lines from the HST FITS files containing observations made using the STIS instrument with either the E140H or the E230H grating.
2 - Continuum Fitting and Normalization: Fit the line-free regions of the continuum around the absorption lines, and normalize the spectrum.
3 - PSF Kernel Creation: Create a custom kernel that incorporates the spectral response of the instrument used (Point Spread Function or PSF).
4 - Simulate Absorption Lines: Simulate absorption lines using information from a line list database such as NIST, MOLAT, or LAMBDA.
5 - Bayesian MCMC Fitting: Fit the simulated absorption lines to the observed lines in the normalized HST spectrum using a Bayesian Markov Chain Monte Carlo (MCMC) approach.

The repository includes the HST data files and PSF files necessary for running the example. The code is works well on a single core when fitting only a few transitions. If fitting multiple bands or numerous transitions, a more robust function for simulating absorption lines will be added to the repository in the near future.

