FROM quay.io/fenicsproject/stable:current
MAINTAINER Mehdi Saraeian <mehdi@iastate.edu>

USER root

ENV DEBIAN_FRONTEND=noninteractive

######################
# Python information #
######################
RUN which python
RUN python -c 'import sys; print(sys.version_info[:])'

######################
# tIGAr Installation #
######################

RUN pip install git+https://github.com/blechta/tsfc.git@2018.1.0
RUN pip install git+https://github.com/blechta/COFFEE.git@2018.1.0
RUN pip install git+https://github.com/blechta/FInAT.git@2018.1.0
RUN pip install singledispatch networkx pulp
RUN pip install git+https://github.com/david-kamensky/tIGAr.git
RUN pip install git+https://github.com/dalcinl/igakit.git
RUN pip install --force-reinstall scipy

#######################
# ShNAPr Installation #
#######################

RUN pip install git+https://github.com/david-kamensky/ShNAPr.git

########################
# VarMINT Installation #
########################

RUN pip install git+https://github.com/david-kamensky/VarMINT.git

###########################
# CouDALFISh Installation #
###########################

RUN pip install git+https://github.com/david-kamensky/CouDALFISh.git
