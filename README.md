# Machine Learning for Chemists

This is a series of notebooks to give you a very quick (circa 24-30 hours) introduction to machine learning, assuming absolutely no python coding experience. It covers *linear regression* in depth using examples from a published paper on cellulose dissolution (allowing the student to repeat the data analysis for a paper). In a tutorial setting with a tutor, this works well as three 3 hours sessions. The unsupervised learning section covers *principal component analysis* (PCA) and clustering algorithms (*k-means*) with an example based on analytical chemistry of wine. The *Supervised learning* section contains a general and brief introduction to neural networks for vision (4_Supervised_learning.ipynb), in order to teach the effects of data set size and some of the problems with neural networks and a section on setting up and using deepchem, moleculenet, rewkit and tensorflow for doing machine learning on chemical problems. (5a_Supervised Learning for Chemistry_a) The supervised and unsupervised sections take about 6-9 hours in a tutorial session (with the lecture note (not yet published, sorry)). 

If you are TECS student, just download the code, unzip and follow the installation instructions below. 

If you are a masters/bachelors student doing a student project with me (hello!), the most important section for you to work through before starting your project is `5a_Supervised Learning for Chemistry_a.ipynb`, then `3a_Unsupervised_Learning_Workbook.ipynb`. When working through `2a_Regression_Cellulose_Workbook.ipynb` you can skip exercises 1 and 4 if you want (or ask me for help). 

## Contents

The notebooks are:
1. `1_Linear_regression.ipynb` very basic intro to linear regression. Work through this.
2. `2a_Regression_Cellulose_Workbook.ipynb` linear regression, including multivariate model fitting, using polynomial features, fitting and overfitting, linearising data and ridge regression. Work through this.
3. `2b_Regression_Cellulose.ipynb` contains example answers. Note that there is more than one method to answer some of the questions.
4. `3a_Unsupervised_Learning_Workbook.ipynb` contains the PCA and clustering examples. Work through this. 
5. `3b_Unsupervised_Learning.ipynb` contains example answers
6. `4_Supervised_learning.ipynb` contains the convolutional neural networks (CNNs) set up with tensorflow for vision tasks (MNIST). Work through this. 
7. `5a_Supervised Learning for Chemistry_a.ipynb` contains the machine learning for chemical problems **work through this!**
8. `5_Supervised Learning for Chemistry_b.ipynb` contains example answers for 5a

## Installation

Download and unzip the code (or use github) and put it into a known directory on your computer (eg. C:\user\My Documents\awesome_code_found_on_the internet\)

**To create a fresh conda environment with the packages you need and start jupyter,**

**for windows:**
if you are using the jupyter suite environment, open that and don't open jupyter lab
instead open the cmd shell.

Into that type the following 3 commands. 
```
conda env create --file .\requirements_win.yml
conda activate ml-for-chemists
jupyter notebook
```
This will install the GPU accelerated version of tensorflow. 
If you don't have a compatible GPU, then edit the appropriate `.yml` file in a text editor and change `tensorflow-gpu` to `tensorflow`.

What this code does:
`conda env create --file .\requirements_win.yml`: creates a new `conda` environment, and loads in the requirements for it and names it ml-for-chemists. This is the easiest way to install the packages you need. 
`conda activate ml-for-chemists`: opens the environment and starts running it. You should see the prompt change from `base` to `ml-for-chemists`
`jupyter notebook`: opens jupyter notebook in a browser for you to start playing with. I recommend chrome.

*If that code doesn't work*
The most likely reason is that you are not in the correct directory. Navigate to the directory in the command window. For example, if you used the stupidly named direcotry above, you would type:
`cd  C:\user\My Documents\awesome_code_found_on_the internet\Machine_learning_for_chemists\`
then 
`jupyter notebook`. 
Or, if `tensorflow` doesn't work, follow the instructions above to change from the gpu version to the standard (`tensorflow`), 

I imagine there is a way to get this running in jupyter lab, but as I haven't got it I haven't tested it, sorry. 

You can open the code in PyCharm instead, just type the commands in the terminal window at the bottom to set up the code. Jupyter notebook files can be run in PyCharm or launched from PyCharm to be run in a separate web-browser window. 

**for linux:**
Put the following in a terminal window. If you don't have a compatible GPU, then edit the appropriate `.yml` file in a text editor and change `tensorflow-gpu` to `tensorflow`.
```
conda env create --file requirements.yml
conda activate ml_for-chemists
jupyter notebook
```

**To run the code once you've installed it**
In windows:
open the Anaconda command window,
navigate to the correct directory (eg. `cd  C:\user\My Documents\awesome_code_found_on_the internet\Machine_learning_for_chemists\`)
then type 
```
conda activate ml-for-chemists
jupyter notebook
```

```
conda env create --file .\requirements_win.yml
conda activate ml-for-chemists
jupyter notebook
```

### Tensorflow 1
For using some datasets, you will need an environment that has tensorflow 1 installed. Using this is much like the other environments, except you need to use the `requirements_tf.yml` file and the resultant environment is called `ml-for-chemists-tf1`. 

**Warning!** Do not run two jupyter instances on the same notebook at the same time.


Currently there is only one tf1 yml file as it should be the same across all platforms.
