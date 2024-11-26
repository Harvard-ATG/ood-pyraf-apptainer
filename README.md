# ood-pyraf-apptainer
This repo is based off of [ood-remote-desktop-rosgazebo](https://github.com/Harvard-ATG/ood-remote-desktop-rosgazebo) and is used to create a remote desktop environment with pyraf, iraf and DS9 packages installed via conda.

## Installation
In order to install the app

Note you will need to be in the head node while building any of the apptainer images.
Apptainer images should be located `/shared/apptainerImages`

- Activate the spack environment and then use activate the apptainer env.
```bash
root@ip:/# . shared/spack/share/spack/setup-env.sh
root@ip:/# spacktivate apptainer
```
- Build the image from the `pyraf.def` file by running `apptainer build pyraf.sif pyraf.def` Note: the `pyraf.sif` should be available in the `/shared/apptainerImages` folder

- After the image is successful you can add the app by following the [Adding OOD app runbook](https://docs.google.com/document/d/1LejSmmgY7rJDBwl1gl-Q835lSbf6v2b2J3TFhxPNwfc/edit?tab=t.0#heading=h.n0uvlxdrj7e3)

