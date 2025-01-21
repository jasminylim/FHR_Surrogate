# FHR Hybrid Surrogate Model for Fluoride-salt-cooled High-temperature Reactor (FHR)

## Decription
The FHR Surrogate Model is a low-complexity model of an FHR system with a gFHR core and a two-loop heat transportation system. This repo contains the work written in the manuscipt *Hybrid Surrogate Modeling Framework for the Digital Twin of a Fluoride-salt-cooled High-temperature Reactor (FHR)* [[1]](https://doi.org/10.1016/j.nucengdes.2024.113690).

## Surrogate Models
* **systemSurrogatePump** : gFHR system surrogate model given the target power 
  * systemSurrogate : gFHR system surrogate with detailed system state
  * systemSurrogatePump : gFHR system surrogate with detailed system state with pump degradation surrogate model

  For usage details, please refer to the [readme](systemSurrogatePump/readme.md).

## Code Tutorials
This repo contains two jupyter notebooks demonstrating the FHR Surrogate Model for a Load Follows case.
  * [```test_LF.ipynb```](systemSurrogatePump/test_LF.ipynb) : Load Follows Case using system surrogate model.
  * [```test_LF_wPump.ipynb```](systemSurrogatePump/test_LF_wPump.ipynb) : Load Follows Case using system surrogate model with pump degradation surrogate model integrated.

These cases are compared with data generated with the [System Analysis Module (SAM)](https://www.anl.gov/nse/system-analysis-module)

## Requirements
Version used during development indicated  
* python3 (3.9.16)
* NumPy (1.26.4)
* Pandas (2.2.2) - for code tutorials
* Matplotlib (3.9.0) - for code tutorials
* Jupyter Notebooks (4.1.6) - for code tutorials

# Quick Guide for Python Environment Setup

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install numpy
pip install pandas 
pip install matplotlib
pip install jupyterlab
```

## Reference
Manuscript: [https://doi.org/10.1016/j.nucengdes.2024.113690](https://doi.org/10.1016/j.nucengdes.2024.113690)