OpenEXR bindings for Python
===========================

Forked from: https://github.com/jamesbowman/openexrpython

Notes on this fork
------------------

This fork fixes the compilation of this Python module to **work with OpenEXR 3.x branch**. It was tested on Linux. Your mileage may vary depending on your system. To use this version, you definitely need one of the latest OpenEXR versions. For instance:
- It replaces the system library names with the new naming scheme
- It replaces `Int64` types to current `uint_64`, `int_64` types.

So, this will *probably* NOT work with earlier versions of OpenEXR, hence not doing a merge request.

Build and install instructions
------------------------------

[![Build Status](https://travis-ci.org/jamesbowman/openexrpython.svg?branch=master)](https://travis-ci.org/jamesbowman/openexrpython)

See homepage at http://www.excamera.com/sphinx/articles-openexr.html

## Requirements

To build from source, a C++ compiler and libraries and development headers for OpenEXR and zlib are required. In Ubuntu, the `g++`, `libopenexr-dev` and `zlib1g-dev` packages suffice all requirements. In OSX, the Homebrew packages `openexr` and `zlib` will suffice.

For the latest release, run:

    pip install openexr

In case the PyPi package is not updated and you want to install from the master branch, you can do the following:

    pip install git+https://github.com/afichet/openexrpython.git

If you prefer, you can clone it and run the `setup.py` file as well. Use the following
commands to get a copy from Github and do the installation:

    git clone https://github.com/afichet/openexrpython.git
    pip install ./openexrpython
