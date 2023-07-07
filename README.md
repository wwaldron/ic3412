# IC 3412

Python pipeline and processing *Hubble Space Telescope* (*HST*) files for IC&#160;3412.

## Various Notes

### Python Environments

Each of the files (with one exception) uses the [`stenv`](https://stenv.readthedocs.io/en/latest/).
As [DeepCR](https://deepcr.readthedocs.io/) can cause conflicts in this environment, an individual
[Deep CR YML file](dcr_env.yml) is provided for that environment. Similarly, the inpainter notebook uses
[Numba](https://numba.readthedocs.io/en/stable/) to speed up the NaN-Median inpainting but this also
conflicts with `stenv`. Therefore, an [Astropy-Numba YML File](astroba.yml) is provided to define
a compatible environment.

### Processing Steps

This repository is only for the Python files needed for processing *HST* files on this galaxy.
The `pipeline` directory houses symbolic links to each of the notebooks used in processing this
galaxy in the order in which they are intended to be run.
