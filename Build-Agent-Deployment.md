Build Agent Deployment 
======================

**Introduction**

Azure DevOps provides developer services to support teams to plan work,
collaborate on code development, and build and deploy applications.
Developers can work in the cloud using Azure DevOps Services or
on-premises using Azure DevOps Server.

Azure DevOps supports adding extensions and integrating with other
popular services, such as: Campfire, Slack, Trello, UserVoice, and more,
and developing your own custom extensions.

**Featured Organization of Services**

Azure DevOps provides integrated features that you can access through
your web browser or IDE client. You can use one or more of the following
services based on your business needs:

-   **Azure Repos** provides Git repositories or Team Foundation Version
    > Control (TFVC) for source control of your code

-   **Azure Pipelines** provides build and release services to support
    > continuous integration and delivery of your apps

-   **Azure Boards** delivers a suite of Agile tools to support planning
    > and tracking work, code defects, and issues using Kanban and Scrum
    > methods

-   **Azure Test Plans** provides several tools to test your apps,
    > including manual/exploratory testing and continuous testing

-   **Azure Artifacts** allows teams to share Maven, NPM, and NuGet
    > packages from public and private sources and integrate package
    > sharing into your CI/CD pipelines.

> Let's follow through a step by step guide to establish the environment
> of a successful CI/CD pipeline and deployment of the projects to a
> virtual machine. There is also a summary of organized URLs at the
> bottom, if preferred to skim through the process.

 Business and Operational Description 
------------------------------------

-   You can set any number of stages during the development and testing
    phases so that you have more control over quality before projects
    move onto the next step.

-   With Azure Pipelines, DevOps teams aren\'t limited to a single
    cloud.

-   Build can be established from open source like GitHub as well as
    other platforms and local machine can also deploy its code using
    Azure Repo.

-   Any changes made to the code are influenced throughout the whole
    environment instantly.

 Build Agent Installation on VM
-------------------------------

A build agent is installed on EC2 instance to create the connection
between the virtual machine and Azure DevOps. This makes it possible for
the pipeline to deploy on that machine. The given links can be used to
navigate to the build agent installation process. Steps are:

-   Create agent pool using:
    <https://devops.ec.va.gov/SharedServices/TestProject/_settings/agentqueues>

![](/Media/BAD1.png)

-   Create build agent using:
    <https://devops.ec.va.gov/SharedServices/TestProject/_settings/agentqueues?queueId=114&view=jobs>

![](/Media/BAD2.png)


-   Download agent on VM and install using PowerShell

![](/Media/BAD3.png)

 
                         
