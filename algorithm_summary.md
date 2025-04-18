# Algorithm Summary

The Toolkit for Extreme Climate Analysis (TECA) Bayesian Atmospheric River Detector (BARD) probabilistic ARDT runs 1,024 separate ARDTs.  Each ARDT has a different choice of relative percentile threshold, tropical filter width, and minimal area; the values for these three parameters were determined using a Bayesian approach that seeks to mimic the detection statistics of eight atmospheric science experts who manually identified ARs in a dataset.  Each of the 1,024 ARDTs produces a `ar_binary_tag` type variable (0 if AR is absent in a grid cell, and 1 if an AR is present); the `ar_probability` field is the average of the outputs of all 1,024 detectors.  A full description can be found in [O'Brien et al. (2020)](https://doi.org/10.5194/gmd-13-6131-2020)

## Documentation

Documentation for running TECA BARD can be found on the [TECA Documentation](https://teca.readthedocs.io/en/latest/applications.html#teca-bayesian-ar-detect) page.  TECA must be installed to use TECA BARD; alternatively, one can use [Docker version of TECA](https://hub.docker.com/repository/docker/obrientaiu/teca_cpu_debug/general) (this is currently experimental and not yet documented) ([TECA, 2023](https://doi.org/10.5281/zenodo.6640287)).

