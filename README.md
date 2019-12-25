# moog_nosm
MOOG without the dependent of SM.

[MOOG](http://www.as.utexas.edu/~chris/moog.html) is a software of generating synthestic spectra and fitting it with observed spectra to get abundances from stellar model and line list. It is written by Chris Sneden.

Original MOOG is related to plotting software [SM](http://www.astro.princeton.edu/~rhl/sm/), which is (maybe) hard to install and call by MOOG. The MOOG in this repository is undependent on SM, so the command MOOG and MOOGSILENT is basically the same.

Beside this some lines are also modified:

- Pi value inside Smooth.f is changed to 3.1415927.
- Some judgement is added to make makefile of MOOGSILENT run normally.
- Input and output format of pixel value of synthetic spectrum inside Binplotprep.f, Smooth.f, Synpop.f, Synspec.f and Vargauss.f is change to f8.4, adding a space between numbers when they are small than 0.
- The output format of Lineinfo.f are modified to output the opacities when `atmosphere` and `lines` are set to 2 and 4.

The modified MOOG of versions NOV2019 and FEB2017 are provided, and their installation methods are identical.

## Install

Here the install method of version NOV2019 are present as example. For the installation of version FEB2017, change `FEB2017` to `NOV2019`.

1. Clone or download the respository.
2. Enter the MOOG folder by `cd PATH_TO_REPO/moog_nosm_NOV2019`.
3. Run the bash file `./install.sh`
4. There will be a prompt asking which kind of machine the installation is on; choose either `Linux` (or simply hit Enter) or `Mac`. I test it in Ubuntu but not for Mac so please be cautious.
5. Then installation should go by itself.
6. If you see some prompt of `make sure that you have entered the proper parameters for MOOG into the FORTRAN source driver routine Moog.f !!!!!!!!!!!!` then you should see a `MOOG` and `MOOGSILENT` file present in the current folder.
7. Done.
