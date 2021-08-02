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

## Contents

This module contains materials to teach machine learning and regression to chemistry students using chemistry relevant examples. No previous python experience is expected. A list of contents for each notebook follows, note that the 'a' notebooks are workbooks for use by the students and the 'b' notebooks contain example answers:

### 1_Linear_Regression:
Teaches basic python and basic linear regression in python (2d line fitting).

### 2_Regression_Cellulose:
Teaching multivariate regression models and model refinement whilst also getting students to redo the data analysis for a paper on using green solvents for cellulose dissolution in organic electrolyte solutions.

### 3_Unsupervised_Learning:
Teaches principal coordinate analysis and clustering algorithms (k-means) and applies these techniques to differentiating wine from different vinyards based on the wine's analytes. 

### 4_Supervised_Learning:
Does not contain any chemistry examples, teaches scoring, dataset size and how ML algorithms can be fooled using pictorial input. 

### 5_Supervised_Learning_for_chemistry
Introduces MoleculeNet and DeepChem. Teaches students how to build and use supervised regression and classification models for chemical problems like determining drug solubility or predicting action against HIV.

## Citation

There will be a paper forthcoming on the application of these tutorials to teach synthetic students digital chemistry.
