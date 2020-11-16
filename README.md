
# Agile Development with Azure - CI/CD

![Alt text](Screenshots/GithubActionsPassedbadge.svg?raw=true "Github Actions Test Passed")
# Overview

This project illustrates the end to end CI & CD using Azure CLI, Github Repository & Actions and Azure Devops Pipeline.
Below are the high level steps.

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
![Alt text](Screenshots/Architecture.PNG?raw=true "Architecture Diagram")


* Project running on Azure App Service
Use the command ```az webapp up -n <app name>``` to run Azure Web App Service
![Alt text](Screenshots/Successful_running_Webapp.PNG?raw=true "Project running on Azure App Service")

* Project cloned into Azure Cloud Shell 

The command ```git clone git@github.com:lalprasad/Udacity-Agile-Dev-with-Azure.git``` is used to clone the remote repo to local.

![Alt text](Screenshots/Successful_cloning.PNG?raw=true "Clone Repo")


* Passing tests that are displayed after running the `make all` command from the `Makefile`
![Alt text](Screenshots/Makefile.PNG?raw=true "make all")

* Successful run of Github Actions
![Alt text](Screenshots/Successful_Github_Actions.PNG?raw=true "Successful run of Github Actions")

* Successful deploy of the project in Azure Pipelines.  
![Alt text](Screenshots/Successful_AzureDevOps_pipeline_run.PNG?raw=true "Build and Deploy via azure devops pipelines")

* Running Azure App Service from Azure Pipelines automatic deployment
![Alt text](Screenshots/Successful_deployment_to_webapp.PNG?raw=true "Running Azure App Service from Azure Pipelines automatic deployment")

* Successful prediction from deployed flask app in Azure Cloud Shell.  

![Alt text](Screenshots/Prediction_results.PNG?raw=true "Successful prediction from deployed flask app in Azure Cloud Shell")


* Output of streamed log files from deployed application
Streamed Logs can be accessed via Azure Portal's Advanced Tools (kudu)

![Alt text](Screenshots/Log_Stream_tail.PNG?raw=true "Kudu")

Also via Azure Portal's Monitoring --> Log Streaming section

![Alt text](Screenshots/LogStream.PNG?raw=true "Log Streaming")

Alternatively Log Stream can can be accessed via CLI using the command

```az webapp log tail --name appname --resource-group myResourceGroup```
![Alt text](Screenshots/LogTraceviaCLI.PNG?raw=true "Log Streaming")

Locust, a popular load testing tool could be used for testing the webapp. Installation steps can be found  [here](https://medium.com/better-programming/introduction-to-locust-an-open-source-load-testing-tool-in-python-2b2e89ea1ff).
Use appropriate values for Number of total users to simulate & Spawn rate (users spawned/second).Below is the screen that shows progress of testing.
![Alt text](Screenshots/Locust_testing_for_azure_web_app.PNG?raw=true "Load testing")




## Enhancements

- Create environments like Breakfix --> Staging --> Production.
- Improve the code review with pull requests so that a reviewer can validate the code (check for errors during merging etc.)
## Demo 

<TODO: Add link Screencast on YouTube>


