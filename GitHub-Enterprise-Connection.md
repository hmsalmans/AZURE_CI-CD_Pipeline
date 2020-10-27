GitHub Enterprise Connection
============================

**1 Introduction**

Azure DevOps provides developer services to support teams to plan work,
collaborate on code development, and build and deploy applications.
Developers can work in the cloud using Azure DevOps Services or
on-premises using Azure DevOps Server.

Azure DevOps supports adding extensions and integrating with other
popular services, such as: Campfire, Slack, Trello, UserVoice, and more,
and developing your own custom extensions.

**2 Featured Organization of Services**

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

3 Business and Operational Description 
--------------------------------------

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

GitHub Repo Access to Fetch the Deployed Project to Create Build
Pipeline:

The link https://github.ec.va.gov/ can be used to deploy a project to
GitHub platform. We can also use the Azure Repo feature if we would like
to deploy the project from our local machine instead.

To create Azure DevOps account, https://azure.microsoft.com/en-us/services/devops/ can be used
.

-   After logging in, A new organization is created.

-   Under this newly created organization, a project is created which
    will have all the features we need to create the CI/CD pipeline.

-   Linking GitHub Repo to Azure DevOps to start building the build
    Pipeline. This is done by creating new build pipeline using Pipeline
    option on left. A new pipeline is created successfully which
    includes the source code from GitHub Repo.

![](media/image5.png)

                         
                         
