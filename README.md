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


## Account Setup

If you do not have Azure DevOps setup you can start for free but you need to sign up using any valid account. Follow below link and start for Free.


https://azure.microsoft.com/en-us/services/devops/?nav=min:

![Cpature](services.png)

# Organization.

Organization is collection of related projects. Also it helps to organize the different Projects.
Once you are signed up there will be Organization created. You can create Multiple Organization with Create New Organization.

![Cpature](orga.png)


# Project
Project helps to build the Software Solution which includes Planning, Tracking,
Source Code Management, Setting Up CI/CD, Releasing Artifact. Once you create Project team will be created Automatically.
Under the Organization you can create Project.

## Create Project
Organization --> New Project --> Create
![projects](orga.png)
![projects](p2.png)

# Azure Repos

Azure Repos helps to create and Manage Source Code which further will be used to Build and Deploy.
For example we can import any sample Project to setup the CI/CD. Use below git repo to import.
![projects](step1.png)
![projects](step2.png)
![projects](step3.png)

#  Azure Pipelines

Once the Source Control setup is completed now we can setup the Continuous Integration and Continuous Deployment

Continuous Integration

Continuous Integration is a process to setup the Build for your application Project, which enables to trigger build pipeline
automatically on each source code Check-In. This helps to track the Build status and and identify build failure caused by specific change.
Lets setup the CI step by Step.


Step :1 Create Build Pipeline

Pipelines --> Create Pipeline
![projects](pipe1.png)


Step 2:  Select the respective repository and the branch.
![projects](pipe2.png)


Step 3:  Create the build using the Classic Editor
![projects](pipe3.png)


Step 4:  Use the ASP.NET Build template since the Sample Repo is ASP.NET web Application.
![projects](pipe4.png)


Step 5: Save the Pipeline and Queue the Build.

![projects](pipe5.png)


Step 6: If you get below error it mean the Free tier is not approved by Microsoft. If you are using MSDN Account you will not receive this error
![projects](pipe6.png)
