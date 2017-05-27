# moog_nosm
MOOG without the dependent of SM.

[MOOG](http://www.as.utexas.edu/~chris/moog.html) is a software of generating synthestic spectra and fitting it with observed spectra to get abundances from stellar model and line list. It is written by Chris Sneden.

Original MOOG is related to plotting software [SM](http://www.astro.princeton.edu/~rhl/sm/), which is (maybe) hard to install and call by MOOG. The MOOG in this repository is undependent on SM, so the command MOOG and MOOGSILENT is basically the same.

Beside this some lines are also modified:
	-Pi value inside Smooth.f is changed to 3.1415927.
	-Some judgement is added to make makefile of MOOGSILENT run normally.
	-Input and output format of pixel value of synthetic spectrum inside Binplotprep.f, Smooth.f, Synpop.f, Synspec.f and Vargauss.f is change to f8.4, adding a space between numbers when they are small than 0. 

Current MOOG version in this repository is February, 2017 version.
