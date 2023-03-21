# Skyline-Starter-Workflows
GitHub starter workflows for DataMiner related development.

We offer a number of starter workflows that can be used as the starting point to create a workflow for your GitHub repository. These .yml files are designed to be small and call both reusable workflows and actions from the marketplace that always try to run the latest versions.

A [GitHub action](xref:Deploying_Automation_scripts_from_a_GitHub_repository) provides an easy access point to a single key action, such as deploying a DMAPP, creating a DMAPP, running tests, and more.

[GitHub reusable workflow](xref:github_reusable_workflows) allows the reuse of a combination of many different GitHub actions and other scripts, running across several jobs combined into a single easy call.

By combining these three concepts, you can avoid maintenance costs and ensure that you always run the latest stable versions without the need for further user configuration. Any default behavior can easily be overwritten and changed on your copy of the starter workflow if you wish to always use a specific version until it is manually adjusted. This might be necessary to meet security requirements for your organization.

## Prerequisite
You require a github organization (that you created or are a member of).
To create a new organization, go to [https://github.com/organizations/plan](https://github.com/organizations/plan) and create a new Organization.

## How to use

Option 1: Individual repository
* You can copy and paste the content of a .yml file from this repository into an Action Workflow of any other Repository.

Option 2 (recommended): Organizations and multiple repositories within it
* Fork this repository into your organization.
  Your fork has a workflow you can activate, this automatically adds starter workflows to your organization and keeps them in-sync (through pull-requests) with ours.
* The workflow requires authentication: You need to create a token under user>settings>developer settings>Personal access tokens (classic)
  * Name: PAT
  * Scopes:
      * repo
      * workflow
      * admin:org/write:org
      * admin:org/read:org
* Run the workflow, and then accept the Pull Request that has appeared on a repository called .github within your organization.
* After the above one-time setup, you will find the Starter Workflows being provided by your organization any time you try to add a new workflow to a repository in your organization.

For more information please see: [https://docs.dataminer.services/develop/CICD/GitHub/GitHub_Starter_Workflows.html](https://docs.dataminer.services/develop/CICD/GitHub/GitHub_Starter_Workflows.html)
