
# PureView AI: An Unbiased NLP Tool For Customer Sentiment

This is team 184's repository to build a tableau dashboard with sentiment and topic modeling allowing users to filter on product attributes, review sentiment, review topic and text contained within user reviews. 

## Data 
https://amazon-reviews-2023.github.io/


# Setup 
Go to GCP Vertex AI > Workbench > Managed notebooks

Create an instance for your personal email

Start the managed notebook then open jupyterlab

On the ribbon above, there is a 'Git' click on that then 'Clone a repository' and paste the link to this repo https://github.gatech.edu/jtriemer3/CSE-6242-Amazon-Review-Sentiment.git

Open terminal and run the below commands

```
source ~/.bashrc
```
###### Create env from yml file - may take some time to download
By using this yml environment we can be sure that we all are sharing dependencies and can run the same code on the same python version 

```
conda env create -f team184-env.yml
```
```
conda activate team184-env
```

NOTE - **Whenever you pip install something new, like pandas, you will need to export the env again (see code below) to overwrite the yml so that we all can share that new package. If you skip this step, the code may not run for everyone due to dependency issues.**

```
conda env export > team184-env.yml
```

###### Creating the conda kernel
This essentially will allow us to use our conda env can be used in a jupyter notebook
```
DL_ANACONDA_ENV_HOME="${DL_ANACONDA_HOME}/envs/team184-env"
python -m ipykernel install --prefix "${DL_ANACONDA_ENV_HOME}" --name team184-env --display-name team184
```
