# Codes for GMX_MMPBSA on HPC & Jupyter/Colab

A workflow/notebook for running GMX_MMPBSA calculations efficiently on High-Performance Computing (HPC) systems and Jupyter/Google Colab — including support for MPI parallel mode and post-analysis code.
We significantly reduce simulation time and simplify free energy calculations (MM/PBSA and MM/GBSA) for GROMACS trajectories. 

## What Is GMX_MMPBSA?
GMX_MMPBSA is a widely used tool that combines GROMACS and APBS for post-processing of molecular dynamics trajectories to estimate binding free energies via MM/PBSA or MM/GBSA methods. However it needs graphical UI to run analysis and it requires a lot dependencies (like conda and amber) to install.

This repository has:

Automated Colab/HPC job submission scripts

MPI support

Google Colab compatibility 

## Usage
- You can open [the notebook](gmx_MMPSA_conda_v0_1.ipynb) or run codes manually
- Mount Google Drive or upload your files
- Set up GMX_MMPBSA
- Run energy decomposition
- Export results to your local system and run gmx_MMPBSA_ana

Using MPI parallelism, this workflow can reduce computation times by 2–8× (depending on system size and HPC specs).

If you use this workflow in your research, please cite for gmx_MMPBSA:

Valdés-Tresanco et al. (2021). gmx_MMPBSA: A New Tool to Perform End-State Free Energy Calculations with GROMACS. J. Chem. Theory Comput. 17, 6281–6291.

Also you can consider citing our Benchmarking analysis:
[Karagöl, T., & Karagöl, A. (2024). Benchmarking GROMACS on Optimized Colab Processors and the Flexibility of Cloud Computing for Molecular Dynamics. bioRxiv, 2024-11.](https://www.biorxiv.org/content/10.1101/2024.11.14.623563v1.abstract) 

