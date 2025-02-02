---

copyright:
  years: 2020, 2022
lastupdated: "2022-11-21"

keywords: troubleshooting for code engine projects, projects, tips for projects, accessing projects, tips for creating project

subcollection: codeengine

content-type: troubleshoot

---

{{site.data.keyword.attribute-definition-list}}

# Debugging projects
{: #troubleshoot-project}
{: troubleshoot}

Use the troubleshooting tips to learn how to troubleshoot {{site.data.keyword.codeengineshort}} projects.
{: shortdesc}

To understand how to create, work with, and delete projects, see [Managing projects](/docs/codeengine?topic=codeengine-manage-project).

## Project limits to consider 
{: #ts-project-limits}

The maximum number of projects that you can create per region is 20. For more information about limits for projects, see [Project quotas](/docs/codeengine?topic=codeengine-limits#project_quotas).

The maximum number of projects includes projects that are active and any projects that are not permanently deleted, such as projects that are soft deleted. A project that is soft deleted can be restored within 7 days before it is permanently deleted. 

When working with the console, review your defined projects from the [Projects page on the {{site.data.keyword.codeengineshort}} console](https://cloud.ibm.com/codeengine/projects){: external}. This listing includes the region where your project lives. From this page, you can delete projects as needed. When you delete a project from the console, the project is soft deleted. The deleted project does not display from the **Projects** page. 

When working with the CLI, use the [**`project list`**](/docs/codeengine?topic=codeengine-cli#cli-project-list) command to display all your projects. The output of this command displays the region where your project lives. 

Use the [**`project delete`**](/docs/codeengine?topic=codeengine-cli#cli-project-delete) command to delete a project. In the CLI, you can delete a project by specifying the name of the project or by specifying the `project id`. If you specify the `--name` of the project, you must be working in the same region where the project lives. If you specify the `--id` of the project, you are not required to be in the same project to issue the **`project delete`** command. 

The following example command soft deletes the `myproject` project so that it can be restored within 7 days, `ibmcloud ce project delete --name myproject -f`. The `-f` option specifies to force the delete without confirmation. Note, this soft deleted project still counts toward the project maximum until the project is permanently removed 7 days later. 

To permanently delete a project so that it cannot be restored, specify the `--hard` option with the [**`project delete`**](/docs/codeengine?topic=codeengine-cli#cli-project-delete) command, for example, `ibmcloud ce project delete --name myproject2 --hard -f`.

For more information, see [deleting a project](/docs/codeengine?topic=codeengine-manage-project#delete-project).



