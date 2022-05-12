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

`python -c "from transformers import pipeline; print(pipeline('sentiment-analysis')('I am hungry'))"`

This downloads a model of around 268 Mb in size for prediction the sentiment. 
The following output is obtained:

`[{'label': 'NEGATIVE', 'score': 0.9992780685424805}]`

# Update (12.05.22)
Since I am now venturing into fulltime into the domain of NLP, with the experience, I can say that a docker based installation always trumps a local install as the dependencies are directly present and the pwd can be easily mounted to work with the existing data.

For transformers with pytorch, head to https://hub.docker.com/r/huggingface/transformers-pytorch-gpu/tags and get a fixed version.
I would also be adding the docker-compose files in this repo
