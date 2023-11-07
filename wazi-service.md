---

copyright:
  years: 2023
lastupdated: "2023-11-07"

subcollection: zmodernization-fscloud

keywords:

---

{{site.data.keyword.attribute-definition-list}}

# Wazi as a Service (WaaS)
{: #waas}

IBM® Wazi as a Service is a solution that enables a cloud native development and test experience for z/OS in IBM Cloud Virtual Private Cloud (VPC). With Wazi as a Service, application developers can develop and test z/OS application components in a virtual infrastructure "as a Service" environment running on IBM Z architecture on IBM Public Cloud. It gives you cloud security, with the ability to scale dynamically by providing on-demand access to z/OS resources where and when you need them, integrated with public cloud services and configured for integration with your existing DevOps tools.

## Key capabilities
{: #key-capabilities}

IBM Wazi as a Service provides the following key capabilities:

- z/OS development and test stock image: You can use the default z/OS stock image to creates and configure a z/OS virtual server instance for development and test in IBM Cloud VPC from the IBM Cloud console.
- IBM Wazi Image Builder: You can create and manage custom images from an existing Z platform by using Wazi Image Builder. It includes a web UI with role-based access and REST APIs to streamline the creation process. You can then deploy the custom images to IBM Cloud VPC to create a virtual server instance.

Then, you can use your industry-standard integrated development environment (IDE) to build, test, and debug your applications.

IBM provides the z/OS dev and test stock image for you to create a virtual server instance.

You can use z/OS dev and test virtual servers only for development, testing, employee education, or demonstration of your applications that run on z/OS. The licensee must not use the Program for production workloads of any kind, or robust development workloads, including without limitation, production module builds, pre-production testing, stress testing, or performance testing.
{: note}

## Stock image
{: #stock-image}

The z/OS dev and test stock image preinstall the products and services. A list of all the available product and services are defined [here](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=vpc-configurations-in-zos-stock-images).

The available versions of the stock image are

- 2.4
- 2.5

## Available regions
{: #available-regions}

You can create z/OS virtual server instances in the following IBM Cloud regions:

| Location                | Region  | 
|-------------------------|---------|
| Brazil (São Paulo)      | br-sao  |
| Canada (Toronto)        | ca-tor  |
| United Kingdom (London) | eu-gb   |
| Japan (Tokyo)           | jp-tok  |
| US East (Washington DC) | us-east |
{: caption="Table 1. Available regions" caption-side="bottom"}


## Storage
{: #storage}

A maximum of 16 TB of block storage is available.

You can create a block storage volume and attach it to your virtual server instance if you want more storage.

You can add multiple storage volumes to accommodate for the required storage.


