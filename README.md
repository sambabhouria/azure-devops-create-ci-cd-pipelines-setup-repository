# LetsDevOps: Introduction to Azure DevOps for Beginners - Create CI/CD Pipelines, Setup Repository

## Introduction

DevOps is a process which helps to enable continuous delivery of value to our end users. Delivery of Software is a process of Planning, 
Developing, Build, Test, Deploy and Retrospective. Azure DevOps gives all these capabilities to achieve the Continuous Delivery under a single platform.


![Cpature](azure-step.png)

## Azure DevOps Components

![Cpature](azure-devops-components.png)


1. Azure Boards

 This component helps to plan your Backlog, Sprint and track it across the team.
![Cpature](boards.png)


2. Azure Repos

This helps to manage the Code Repository with unlimited private Git Repo. It can be integrated with Centralized [TFS] as well as decentralized [Git] repository with Source Code Management 
![Cpature](repos.png)

3. Azure Pipelines

This is very important feature for the DevOps practice. Azure Pipelines helps to setup the  [CI/CD] 
Continuous Integration and Continuous Deployment. The beauty of this component is that it can be used for any platform like Windows, Linux, Mac OS as well as with any Cloud provider.

![Cpature](piplines.png)

4. Azure Test Plans

This component helps to integrate the TestPlans for your application to validate the changes before shipping to the Customer.

![Cpature](tests.png)

5. Azure Artifact

Azure Artifact helps to create package which can be shared by different Teams also this can be integrated with CI/CD pipeline.
![Cpature](artifacts.png)








### What is YAML

YAML is a human-readable data-serialization language and it helps to configure pipeline as a Code.
The page will reload when you make changes.\
You may also see any lint errors in the console.

`Indentation is very important in YAML.`

## YAML Pipeline

In Azure DevOps, Pipelines helps to setup Continuous Integration/ Continuous Deployment and to achieve
this we have below two option .

1. Classic Editor.
2. YAML Pipeline.

In this Document we will discuss setup YAML Pipeline.
# YAML Pipeline Structure 

![https://github.com/sambabhouria/complete-guide-to-learn-and-setup-yaml-pipeline-in-azure-devops](Yaml-pipeline-structure.png)

# Hierarchy of YAML File


# Component of YAML Pipeline
Here is the list of component which we use in YAML pipeline creation.

1. Stages.
Stage is collection of Jobs which runs sequentially.

![https://github.com/sambabhouria/complete-guide-to-learn-and-setup-yaml-pipeline-in-azure-devops](stages.png)

2. Jobs.
Job is Collection of Steps that runs on agents/environment.
![https://github.com/sambabhouria/complete-guide-to-learn-and-setup-yaml-pipeline-in-azure-devops](jobs.png)


3. Steps.
Steps helps to define the set of process to setup your task or any activity which you want to perform on any specific job.

Kind of Steps
+ `Task`
+ `Script`
+ `templatereference`
![Cpature](steps.png)

# Schema of YAML Pipeline file.

![Cpature](schema-of-pipeline-file.png)

# `Important Note:-`

1.In some cases if there is only one stage required for pipeline we can omit stage keyword and can directly start from Jobs.

2. In some build setup where only one agent is required for pipeline in that case we can omit Job and directly define the Steps.

# DEMO:
We can begin with demo to setup YAML pipeline for below three scenarios.

`Single Stage, Single Job YAML Pipeline`
`Single Stage Multi Job YAML Pipeline`
`Multi Stage YAML Pipeline`


1. Single Stage, Single Job YAML Pipeline

Assume that if you have assigned to setup build for an application. In this scenario we can omit stages or Jobs.
![https://github.com/sambabhouria/complete-guide-to-learn-and-setup-yaml-pipeline-in-azure-devops](single-stage-single-job.png)

Here you can notice that we did not include the Stage and Job section  in the YAML pipeline as it is not required in this scenario.

2. Single Stage Multi Job YAML Pipeline

Let's assume you have to perform some activity on different Agent. Like building application on Windows, Mac OS, Linux. In this scenario we can create multiple job and each job can be assigned with respective agent.
![https://github.com/sambabhouria/complete-guide-to-learn-and-setup-yaml-pipeline-in-azure-devops](single-stage-multi-job.png)


3. Multi Stage YAML Pipeline.

In this scenario you have assigned one application where you need to build the Project, package it. After that you need to deploy the application. In this case we can create two stage.

Stage1 --> Build the Application
Stage 2 --> Deploy the Application
![https://github.com/sambabhouria/complete-guide-to-learn-and-setup-yaml-pipeline-in-azure-devops](multi-stage-multi-job.png)


For more watch this video

[YAML Pipeline Tutorial](https://www.youtube.com/watch?v=JtbG6WkLGng&ab_channel=SumitRaj)
