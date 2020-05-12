# TIPS FOR USING CONDA

## INSTALLATION (WINDOWS)
Install from browser using the default options: https://docs.anaconda.com/anaconda/install/windows/

Open the **Anaconda Command Prompt** and update the base version of conda
- run to check version: `conda --version` and `python --version` to check versions
- run to update `conda upgrade conda` then `conda upgrade --all`

Don't install new packages into base, if a new environment is required follow the steps below


## ENVIRONMENTS
create new environment: `conda create -n [name_here] python=3`

access new environment: `source activate [name_here]`

install packages: `conda install numpy pandas matlab`

install jupyter: `conda install jupyter notebook`

view installed pacakages: `conda list`

save environment to a .YAML file: `conda env export > environment.yaml`

create environment from .YAML file: `conda env create -f environment.yaml`

exit an environment: (OSX/Linus) `conda deactivate`, (Windows) `deactivate`

remove an environment: `conda env remove -n env_name`


## USING IN GIT BASH FOR SCRIPTING
Install Git with Unix tools: https://git-scm.com/download/win 

Open Git Bash

Add python to PATH:
- to get PATH: `pwd`
- add to path: `echo 'export PATH="$PATH:[YOUR_PATH]/anaconda3:[YOUR_PATH]/anaconda3/Scripts"' >> .bashrc`
- create alias: `echo 'alias python="winpty python.exe"' >> .bashrc`

