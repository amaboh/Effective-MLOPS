# Effective-MLOPS for Machine learning

#### Overview
This is an implementation of CI/CD in an ML project using GItOps and Experiment tracking. The focus is on utilizing GitHub Actions to enforce and automate certain policies and Weights & Bias to generate reports on model runs. 

### Motivation
This project is the result of me taking the weights and bias course on Ci/CD for MLOPs and reading and digging more about MLOPs and realizing I'll like to help others have a resource which they can refer too when trying to learn about. You can find a complete blog post about this on [Medium](https://medium.com/@amaboh/understanding-ci-cd-for-machine-learning-when-shipping-models-into-production-44341e4aaa41)


#### File structure 
.github/workflows: contains all GitHub Actions workflows files.
/data: Train and testing data
/notebooks: Notebooks for model development and expirement.
/source/tests: python scripts to geenrate reports, tests etc
requiremnts.txt

### How to install and run project
- Fork this repository
- Clone your forked repository
- create Wandb account get API keys
- Use Wand credentials in the notebook and run notebook
- Create secret for Wandb Api key 
- Commit and push with comment '/wandb <run id>

### How to use the project to setup your CI/CD workflow
- Copy the workflow in .github/workflows folder and edit accord to your desired workflow
- Copy model_report.py to generate report
