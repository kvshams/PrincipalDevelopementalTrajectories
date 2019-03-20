# Principal Developemental Trajectories Estimation

## Contents

- [Overview](#overview)
- [Repo Contents](#repo-contents)
- [System Requirements](#system-requirements)
- [Issues](https://github.com/BiascoLab/PrincipalDevelopementalTrajectories/issues)
- [Citation](#citation)
# Overview

This is a R implementation of the  structure-aware algorithm aimed to at revealing and consolidating continuous, low-dimensional and high- density structures in the underlying higher-dimensional data, while ignoring noise and outliers. The theory, proof of convergence to the exact underlying data manifolds (under Gaussian noise assumption) and a deep investigation of its performance under different scenario can be found in Wu, Shihao, et al. [Wu, Shihao, et al. "Structure-aware Data Consolidation." IEEE transactions on pattern analysis and machine intelligence (2017)]
# Repo Contents

- [PrincDevelTraj.R](./PrincDevelTraj.R): `R` script.
- [coordinates_sorted_HSPC_dataset.txt](./coordinates_sorted_HSPC_dataset.txt): Force-directed layout generated by means of SPRING for sorted HSPC dataset.
- [coordinates_CD34_CD164_dataset.txt](./coordinates_CD34_CD164_dataset.txt): Force-directed layout generated by means of SPRING for sorted HSPC dataset.

# System Requirements

## Hardware Requirements

The script requires only a standard computer with enough RAM (>4Gb) to analyze a dataset with 10K obs. in a 2-dimensional space.
The runtimes on provided datsets is approximately 4 minutes.

## Software Requirements
The script had been developed and tested on R version 3.4.x
### Package dependencies

Users should install the following packages prior to run  `PrincDevelTraj.R`, from an `R` terminal:

```
install.packages(c('RANN', 'parallel'))
```

# Reproducibility

To reproduce results published in our paper set parameters with the following values:
- coordinates_sorted_HSPC_dataset.txt -> radius= 0.05; mu= 0.3; 
- coordinates_CD34_CD164_dataset.txt -> radius= 0.02; mu= 0.3; 

