
![Alt text](Screenshots/Github Actions Passed badge.svg?raw=true "Github Actions Test Passed")
# Overview

This project illustrates the end to end CI & CD using Azure CLI, Github Repository & Actions and Azure Devops Pipeline.
Below are the high level steps 

- Create Github Repo
- Create Cloud Shell environment
- Clone Github repo on cloud shell
- Add Github Actions to the repo
- Create Azure Pipeline

## Project Plan
A project plan defines project goals and objectives, specifies tasks and how goals will be achieved, identifies what resources will be needed and associated budgets and timelines for completion

* [Link Project Plan Google Sheets](https://docs.google.com/spreadsheets/d/1aA0WSXAc28xzMDn904-toVYe_riCKqmD7kQ_-z7ctaQ/edit?usp=sharing).
* [Link Project Plan Trello Board](https://trello.com/b/YhWFEYlw/udacity-ci-cd-project).

## Instructions

<TODO:  
* Architectural Diagram (Shows how key parts of the system work)>

<TODO:  Instructions for running the Python project.  How could a user with no context run this project without asking you for any help.  Include screenshots with explicit steps to create that work. Be sure to at least include the following screenshots:

* Project running on Azure App Service

* Project cloned into Azure Cloud Shell 
![Alt text](Screenshots/Successful_cloning.PNG?raw=true "Clone Repo")


* Passing tests that are displayed after running the `make all` command from the `Makefile`
![Alt text](Screenshots/Make file.PNG?raw=true "make all")

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

- Create environments like Breakfix --> Staging --> Production.
- Improve the code review with pull requests so that a reviewer can validate the code (check for errors during merging etc.)
## Demo 

<TODO: Add link Screencast on YouTube>


