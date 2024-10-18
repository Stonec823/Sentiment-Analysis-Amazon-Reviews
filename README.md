
# PureView AI: An Unbiased NLP Tool For Customer Sentiment

This is team 184's repository to build a tableau dashboard with sentiment and topic modeling allowing users to filter on product attributes, review sentiment, review topic and text contained within user reviews. 

## Data 
https://amazon-reviews-2023.github.io/


# Setup 
go to GCP Vertex AI > Workbench > Managed notebooks
create a managed notebook for your personal email, I made one with 30 GB of memory
start the managed notebook then open jupyterlab

on the ribbon above, there is a 'Git' click on that then 'Clone a repository' and paste the link to this repo https://github.gatech.edu/jtriemer3/CSE-6242-Amazon-Review-Sentiment.git

open terminal and run the below commands

```
source ~/.bashrc
```
###### Create env from yml file - may take some time to download
```
conda env create -f team184-env.yml
```

###### Add the conda kernel.  
```
DL_ANACONDA_ENV_HOME="${DL_ANACONDA_HOME}/envs/team184-env"

python -m ipykernel install --prefix "${DL_ANACONDA_ENV_HOME}" --name team184-env --display-name team184
```
