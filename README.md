# Introduction to NLP Course Notebooks
This repository contains Jupyter notebooks for hands-on Natural Language Processing projects.

## Installed Packages
These are the installed packages and versions used for the various projects. All were installed in a conda environment (see below for how I created this).

python=3.11

```
nltk==3.9.1 
pandas==2.2.3 
matplotlib==3.10.0 
spacy==3.8.3 
textblob==0.18.0.post0 
vaderSentiment==3.3.2 
transformers==4.47.1 
scikit-learn==1.6.0 
gensim==4.3.3 
seaborn==0.13.2 
torch==2.5.1 
ipywidgets==8.1.5
```

## Conda Environment
Virtual environments are a great way to manage different packages for different projects. Creating a virtual environment for this particular set of projects allows you to ensure you can use the correct packages without affecting any other packages you already have installed.

```
conda create --name intro_to_nlp_env python=3.11
conda activate intro_to_nlp_env
pip install nltk==3.9.1 pandas==2.2.3 matplotlib==3.10.0 spacy==3.8.3 textblob==0.18.0.post0 vaderSentiment==3.3.2 transformers==4.47.1 scikit-learn==1.6.0 gensim==4.3.3 seaborn==0.13.2 torch==2.5.1 ipywidgets==8.1.5
python -m spacy download en_core_web_sm
pip install ipykernel jupyterlab notebook
python -m ipykernel install --user --name=intro_to_nlp_env
```
Then, when in the notebook, remember to check the kernel is set to "nlp_course_env".
