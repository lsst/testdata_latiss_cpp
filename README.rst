###################
testdata_latiss_cpp
###################

``testdata_latiss_cpp`` is a package in the `LSST Science Pipelines <https://pipelines.lsst.io>`_.

.. This package supplies a set of exposures to test the construction and use of calibration products with the `ci_cpp`_ package.

.. _ci_cpp: https://github.com/lsst/ci_cpp_gen3/

Contents of this package
------------------------

This package contains a number of exposures in the ``raw/`` directory, along with a ``manifest.yaml`` file that maps the exposure IDs of the raw exposures to their purpose in the `ci_cpp`_ package.  For example, a combined bias will be constructed from the exposures listed in the ``biasExposures`` list entry.

Using this package
------------------

This package is designed to be used in conjunction with the `ci_cpp`_ package, which contains the commands to ingest and process these file.  This testdata package must be set up first, using commands like:

  $ cd PATH_TO_TESTDATA_LATISS_CPP
  $ setup -r .
  $ cd PATH_TO_CI_CPP_GEN3
  $ setup -kr .

Package documentation: https://pipelines.lsst.io/packages/testdata_latiss_cpp

Git LFS
-------

To clone and use this repository, you'll need Git Large File Storage (LFS).  The full package will use about 11GB of disk space.

Our [Developer Guide](https://developer.lsst.io/tools/git_lfs.html)
explains how to set up Git LFS for LSST development.

