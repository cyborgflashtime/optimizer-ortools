optimizer-ortools
===================

Compute an optimized solution to the Vehicle Routing Problem with Time Windows and various constraints using OR-Tools.
This wrapper is designed to be called through [Optimizer-API](https://github.com/Mapotempo/optimizer-api) and has been tested on Ubuntu 17.10, 18.04. Linux Mint 18, Debian 8.

Installation
============
## Requirements

Require OR-Tools for the C++ part. Fetch source code at [https://github.com/google/or-tools](https://github.com/google/or-tools).

The current implementation has been tested with the version 6.5 of OR-Tools

    git clone git@github.com:google/or-tools.git
    git fetch
    git checkout tags/v6.5 -b v6.5

    sudo apt-get install git bison flex python-setuptools python-dev autoconf \
    libtool zlib1g-dev texinfo help2man gawk g++ curl texlive cmake subversion

    make third_party

    make cc

More details on [Google Optimization Tools Documentation](https://developers.google.com/optimization/introduction/installing)


## Optimizer

Compile the C++ optimizer

    make tsp_simple
