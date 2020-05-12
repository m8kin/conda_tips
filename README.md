# TIPS FOR USING CONDA

## INSTALLATION (WINDOWS)
Install from browser using the default options: https://docs.anaconda.com/anaconda/install/windows/

Open the **Anaconda Command Prompt** and update the base version of conda
- run to check version: `conda --version` and `python --version` to check versions
- run to update `conda upgrade conda` then `conda upgrade --all`

Don't install new packages into base, if a new environment is required follow the steps below

## SETUP NEW ENVIRONMENT
create new environment: `conda create -n [name_here] python=3`

access new environment: `source activate [name_here]`

install packages: `conda install numpy pandas matlab`

install jupyter: `conda install jupyter notebook`

view installed pacakages: `conda list`
