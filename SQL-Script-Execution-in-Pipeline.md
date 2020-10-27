SQL Script Execution in Pipeline
================================

Version 1.0

October 16, 2020 \| Enterprise Cloud Solutions Office (ECSO)

FOR INTERNAL USE ONLY

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

4 Release Pipeline Process 
--------------------------

Steps are:

-   After the build pipeline is created, the release pipeline can be
    started. First the artifacts are established based on build
    pipeline. The artifacts take the code and transfer it to zip file
    and save them.

![](/Media/SSE1.png)

-   Then staging in initiated from that artifact. As the stage has a zip
    file, which needs to be unzipped, an extract file task is added as
    well.

![](/Media/SSE2.png)

-   Afterwards, an SQL Command task is added to run the SQL script
    successfully.

-   Microsoft SQL server have to be installed on
    the build agent server and SQLCMD utility should be installed as
    well to run the SQL Command.*

![](/Media/SSE3.png)

-   The script is run successfully as it brings the artifacts in the
    logs as well as a new file can be generated automatically using that
    script.

-   

![](/Media/SSE4.png)

![](/Media/SSE5.png)

**5 Summary for Quick Establishment of The Environment**

-   GitHub Repo Deployment

<https://github.ec.va.gov/>

-   Azure DevOps Portal

<https://devops.ec.va.gov/>

-   Agent Pool Creation

<https://devops.ec.va.gov/SharedServices/TestProject/_settings/agentqueues>

-   Agent Download and Installation

<https://devops.ec.va.gov/SharedServices/TestProject/_settings/agentqueues?queueId=114&view=jobs>

**6 User Notification**

A user can be notified as the builds proceed along. Build, release,
success, failure, and code updates are the some of many notifications
that can be triggered once an event happens. Project settings option at
the bottom takes us to the page where the notification methods can be
stored. You can send notifications to an individual email or a team
member.

![](/Media/SSE6.png)

7 Support Escalation Paths {#support-escalation-paths .list-paragraph}
--------------------------

The information below provides the contacts for support escalation.

### Vendor Supports

### VA Support

### Key Contacts, Websites Portals

                         
