# Overview

This project will show you how to set up Continous Integration with Github Actions and Continous Deployment with Azure Pipelines

## Project Plan

* [Link to a Trello board for the project](https://trello.com/invite/b/2dIg2sPk/f0fa24041f7b13471b794dacd36ffaac/flask-ml-service)
* [Link to a spreadsheet that includes the original and final project plan](https://docs.google.com/spreadsheets/d/1H4LCgfTe1PfxhTLpWj3LwC1k_zB-vXn9TTgFLwmq2rA/edit?usp=sharing)

## Continuous Integration with Github Actions
This project is living on ```github-actions``` branch. It is just a simple project to demo CI by using Github Actions

* Architectural Diagram
![Architectural Diagram](./images/ci-diagram.png)

### Instructions


## Instructions
* Create a ssh keypair and put it into your github, and then clone your repo by using ssh authentication
![Github repo was cloned by using ssh key](./images/github_repo_was_cloned.png)

* Checkout into a new branch ```git checkout -b github-actions```
* Copy following files from my repo:
```bash
|__Makefile
|__hello.py
|__test_hello.py
|__requirements.txt
```
* Test and verify output of testing by running command ```make all```
![Output of passing test run](./images/make_all_test_passed.png)
* Push your changes to your repo
```bash
git add .
git commit -m "init source code"
git push --set-upstream orgin github-actions
```
* Enable Github Actions on your repo

<TODO:  
* Architectural Diagram (Shows how key parts of the system work)>

<TODO:  Instructions for running the Python project.  How could a user with no context run this project without asking you for any help.  Include screenshots with explicit steps to create that work. Be sure to at least include the following screenshots:

* Project running on Azure App Service

* Project cloned into Azure Cloud Shell

* Passing tests that are displayed after running the `make all` command from the `Makefile`

* Output of a test run

* Successful deploy of the project in Azure Pipelines.  [Note the official documentation should be referred to and double checked as you setup CI/CD](https://docs.microsoft.com/en-us/azure/devops/pipelines/ecosystems/python-webapp?view=azure-devops).

* Running Azure App Service from Azure Pipelines automatic deployment

* Successful prediction from deployed flask app in Azure Cloud Shell.  [Use this file as a template for the deployed prediction](https://github.com/udacity/nd082-Azure-Cloud-DevOps-Starter-Code/blob/master/C2-AgileDevelopmentwithAzure/project/starter_files/flask-sklearn/make_predict_azure_app.sh).
The output should look similar to this:

```bash
udacity@Azure:~$ ./make_predict_azure_app.sh
Port: 443
{"prediction":[20.35373177134412]}
```

* Output of streamed log files from deployed application

> 

## Enhancements

<TODO: A short description of how to improve the project in the future>

## Demo 

<TODO: Add link Screencast on YouTube>


