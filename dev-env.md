---

copyright:
  years: 2023
lastupdated: "2023-11-07"

subcollection: zmodernization-fscloud

keywords:

---

{{site.data.keyword.attribute-definition-list}}

# Development environment
{: #development-environment}

## Developing with IBM Wazi for development spaces
{: #dev-wazi-dev-spaces}

IBM® Wazi for Dev Spaces provides the z/OS® application development capabilities in the OpenShift® Container Platform environment. After the cluster administrator of your organization completes the installation, each z/OS application developer on the team can create a development workspace. Then, the z/OS application developer can edit, build, and debug mainframe applications from any machine without any local environment configurations.

## Requirements
{: #reqs}

- Ensure that you have a connection to a Red Hat® OpenShift Container Platform cluster, and that you have cluster-admin permissions.
- Install the Red Hat OpenShift command line interface (CLI), which you can use to create applications and manage OpenShift Container Platform projects from a terminal.

### Storage
{: #storage}

A storage strategy describes how a workspace uses persistent volume claims (PVCs) and persistent volumes (PVs). Storage is for workspace data, such as projects, workspace logs, or additional volumes defined by a user.

| Storage strategy name | common                                                                                 | per-workspace                                | unique                     |
|-----------------------|----------------------------------------------------------------------------------------|----------------------------------------------|----------------------------|
| PV count              | One per user                                                                           | One per workspace                            | Multiple PVs per workspace |
| Default               | yes                                                                                    | no                                           | no                         |
| Limitations           | Maximum one running workspace per user when the PV is in the ReadWriteOnce access mode. | PV count depends on the number of workspaces. | Unpredictable PV count     |
{: caption="Table 1. Storage strategy" caption-side="bottom"}

