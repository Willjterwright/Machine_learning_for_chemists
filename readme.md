# Machine Learning for Chemists

## Installation

To create a fresh conda environment with the packages you need and start jupyter,
for linux:

```
conda env create --file requirements.yml
conda activate ml_for_chemists
jupyter notebook
```

for windows:
```
conda env create --file .\requirements_win.yml
conda activate ml_for_chemists
jupyter notebook
```

Substitute whatever you like for `ml_for_chemists`. This will install the GPU accelerated version of tensorflow. 
If you don't have a compatible GPU, then edit the appropriate `.yml` file in a text editor and change `tensorflow-gpu` to `tensorflow`.
