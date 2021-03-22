# Machine Learning for Chemists

## Installation

To create a fresh conda environment with the packages you need and start jupyter:

for windows:
```
conda env create --file .\requirements_win.yml
conda activate ml-for-chemists-tf2
jupyter notebook
```

for linux:

```
conda env create --file requirements.yml
conda activate ml-for-chemists-tf2
jupyter notebook
```

This will install the GPU accelerated version of tensorflow. 

If you don't have a compatible GPU, then edit the appropriate `.yml` file in a text editor and change `tensorflow-gpu` to `tensorflow`.
