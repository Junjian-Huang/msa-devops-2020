# msa-devops-2020


deployed website on Azure:
https://msa-2020-devop.azurewebsites.net



Karim-C GitHub invite link:
https://github.com/Junjian-Huang/msa-devops-2020/invitations


Paulvtan GitHub invite link:
https://github.com/Junjian-Huang/msa-devops-2020/invitations


Build Pipeline:

-I created a pipeline organization on Azure DevOps and connected to a GitHub repository. Azure DevOps will automatically create a YAML file for you or you can manually create YAML file on your local GitHub. This is a main file to defines the pipeline, you can set up triggers, scripts, steps etc. in this file. After you set up functions on YAML file, each time you synchronise a push commit to the master branches in your GitHub repository the pipeline will be run. When I finished to configurate my pipeline, Azure stared up a job to run the pipeline. The job responsible to checkout version, testing and provide information with for debugging etc.


Release Pipeline:

-I created a Build Pipeline and I need to use Release Pipeline to deploy the Build Pipeline (artifact). Release Pipeline responsible for taking care of build artifact from build pipeline. In this function, I could choose to use which Azure app service to deploy my artefact. I also could specify which build branch that could be deployed. For example, there are two commit branches in my artefact. I only want the master branch continuous to be deployed. When I commit some change to sub-branch, it would not affect the master branch which is deploying on release pipeline. 
