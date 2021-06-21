# Transformers

Python | PyTorch | Transformers 
Intro to transformers with Hugging Face

Starting with NLP by using the tutorial provided by Hugging Face.

Using the Transformers library provided by Hugging Face, which has pretrained models concerning the tasks on texts. 


## Local Setup

In order to not use the Google Colab, but use the local PC for executing the code on the Jupyter Notebook, it is necessary to follow these steps.(Since my PC has already setup with all the libraries required for Deep Learning, the following extra steps were taken by me)

Since I use Conda for managing the python environments, I need to install transformers using conda. Activate the conda environment and then install transformers.
  
` conda install -c huggingface transformers`

To check the installation:

`python -c "from transformers import pipeline; print(pipeline('sentiment-analysis')('we love you'))"`

This downloads a model of around 268 Mb in size for prediction the sentiment. 
The following output is obtained:

`[{'label': 'POSITIVE', 'score': 0.9998704791069031}]`
