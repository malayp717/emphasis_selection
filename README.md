# Emphasis Selection For Written Text in Visual Media

## Installation
```
git clone https://github.com/malayp717/emphasis_selection.git
cd emphasis_selection
virtualenv project
pip install -r requirements.txt
```

Note: If not having virtualenv, install it using: `pip install virtualenv`.
Download pre-trained GloVe embeddings from `http://nlp.stanford.edu/data/glove.6B.zip`

## Problem Statement
The problem statement ([Task 10 in SemEval-2020](https://competitions.codalab.org/competitions/20815)) is designing automatic methods for emphasis selection i.e. choosing candidates for emphasis in short written text.

More formally,
Given a sequence of words or tokens C = $\{x_1, x_2, ..., x_n\}$, we want to compute a score $S_{i}$ for each $x_{i}$ which indicates the degree of emphasis to be laid on the word.

## Directory Structure
- datasets $\rightarrow$ contains the train and development sets

- BiLSTM_Attention_approach $\rightarrow$ contains the model for 'BiLSTM + Attention' approach

- Transformers_approach $\rightarrow$ contains model and ensemble files for Transformers approach

- requirements.txt $\rightarrow$ contains versions of packages required

- eval_metric.py $\rightarrow$ contains the function for Match $_{m}$ as defined in task
