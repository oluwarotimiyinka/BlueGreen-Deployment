# Introduction 
This is a continous deployment project of .Net App in Azure Web Service with production and devlopment Slots.
The App can be swapped between the two sots.

# STEPS
1.	Create a new project project in Azure DevOps and initiated a new git repository with README file.
2.	Deploy new Azure linux App service
3.	Create and run a new yaml pipeline with bash commands to install and deploy DotNet 8.0 to the App Service.
4.	Initiate a new repository in VS code or GitHub code spaces
5.	Create a new branch in the VS code git with the name development
6.	Create a folder within the development and deploy new DotNet8.0 App into the new folder
7.	Clone the Azure DevOps repository into Vs code repository
8.	Add the development branch to the remote git, commit and push
9.	In Azure portal, create development slots in App Service and label the new slot "green"
10.	In Azure DevOps, clone a new pipeline from main pipeline in development branch
11.	Comment out the DotNet install bash command and add AzureAppServicemanageer to configure Slot Swaps
12.	Run the pipeliness
13.	Add branch policy and validation to the development branch
14.	Resolve merge conflicts in VS code, merge the development and main branch in Azure DevOps to effect the slots swap.

# Outcome

VS Code Merge Conflicts
<img src= "https://github.com/oluwarotimiyinka/BlueGreen-Deployment/blob/main/Screenshot%202024-11-28%20024318.png" alt="VS Code Merge Conflicts" width="350" height="350">

Swapped Slot
<img src= "https://github.com/oluwarotimiyinka/BlueGreen-Deployment/blob/main/Screenshot%202024-11-28%20130257.png" alt="VS Code Merge Conflicts" width="350" height="350">

# Challenge
Resolving the conflicts while merging the development repository with the main repository from Azure DevOps was challenging.
Visual Studio Code conflict editor was used for the merging the changes, and the repository was sychnonized with Azure DevOps repositores before the final merge in Azure DevOps
