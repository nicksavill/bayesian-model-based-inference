# Introduction #

Bayesian model based inference. Fit nonlinear dynamical mathematical models to multivariate time series data using a Bayesian framework. This software has only been tested on Linux.


# Installation #

In addition to this code you will need

1) Intel® C++ Composer XE 2013 for Linux which can be downloaded from

http://software.intel.com/en-us/non-commercial-software-development

Don't forget to add the following to your .bashrc or .bash\_aliases

. /opt/intel/bin/compilervars.sh intel64

2) grace which you can download from

http://plasma-gate.weizmann.ac.il/Grace/

or it may be available on your linux distribution

3) GNU R standalone mathematics library available for your distribution (in particular Rmath.h and libRmath.so).

4) GNU Scientific Library (GSL) available for your distribution.


First enter the Bayes/Python/pygrace-0.3 directory and, as root, type

python setup.py install

Add the following to your bash profile (.bash\_profile or .profile files)

PATH=$PATH:$HOME/Bayes/Python
export KMP\_AFFINITY=compact


Download bayes.tgz and model.tgz into your home directory. Uncompress with

tar xzf bayes.tgz
tar xzf model.tgz

# Compilation and Running #

cd into the PLoS directory and type

make

then run the simulation with the command

./ba1