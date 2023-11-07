---

copyright:
  years: 2023
lastupdated: "2023-11-07"

subcollection: zmodernization-fscloud

keywords:

---

{{site.data.keyword.attribute-definition-list}}

# z/OS Connect
{: #z-os-connect}

## Creating REST APIs to access existing applications and data
{: #rest-apis}

The use of REST APIs for z/OS has matured as a key mechanism for modernizing and unlocking the value of existing applications and data. With this maturity has grown the number and diversity of development teams engaging with the mainframe. This requires a development and deployment model that supports agility and enables self-service provisioning.

IBM z/OS Connect includes cloud native development support and API first mapping for creating OpenAPI 3 interfaces to z/OS applications and data. To achieve this, we have added two new components; a new container-based deployment model that is known as the IBM z/OS Connect server and a powerful new browser-based tooling that is known as the z/OS Connect Designer.

![overview](image/zconnect-overview.svg){: caption="Figure 1. The z/OS Connect OpenAPI3 provider experience" caption-side="bottom"}

## Calling APIs from CICS COBOL applications
{: #apis-cics}

From V3.0.65, generating and deploying API requesters by using the IBM z/OS Connect API requester Gradle plug-in, CICS COBOL applications can call APIs that conform to the OpenAPI 3.0 specification.

To call APIs, you generate and deploy API requesters into IBM z/OS Connect. An API requester is created by generating the artifacts for an API requester that uses the API requester Gradle plug-in and an OpenAPI 3.0 definition. The IBM z/OS Connect API requester support is applicable to z/OS Connect native server.

Figure 2 shows how the IBM z/OS Connect API requester uses the Host API to allow z/OS applications to call API endpoints.

![arch](img/requester-end-to-end-export.svg){: caption="Figure 2. The z/OS Connect OpenAPI3 requester experience" caption-side="bottom"}

## System requirements
{: #system-reqs}

Detailed system requirements to run IBM z/OS Connect (OpenAPI 3), either as a native server on z/OS or as an image in an OCI-compliant container platform.

### Hardware requirements
{: #hardware-reqs}

IBM z/OS Connect runs on any hardware that supports the chosen operating system.

**z/OS Connect Designer**

* Currently available on s390x and amd64 architecture.

**z/OS Connect server**

* Currently available on s390x and amd64 architecture.

### Software requirements
{: #software-reqs}

**z/OS Connect Designer**

An OCI-compliant container runtime of your choice, for example, Docker Desktop V19.0.3 or later.

**API provider Gradle plug-in**

* API provider Gradle plug-in V1.0 to V1.0.2 supports Gradle V6.8.3 to V8.0.2.
* API provider Gradle plug-in V1.1.0 and later versions supports Gradle V7.6.1 to V8.1.

**API requester Gradle plug-in**

* API requester Gradle plug-in V1.0 to V1.0.2 supports Gradle V6.8.3 to V8.0.0.
* API requester Gradle plug-in V1.0.3 and later versions supports Gradle V7.6.1 to V8.1.

**z/OS Connect server**

An OCI-compliant container platform of your choice, for example, Red Hat OpenShift V4.9 or later.

**z/OS Connect native server**

* z/OS V2.4 or later.
* IBM z/OS Connect V3.0.55 or later.
* IBM 64-bit SDK for z/OS.

**DevOps**

* Supported Gradle release depends on release of Gradle plug-in in use for API provider and API requester.
* Java™ Technology Edition V8.0.0 or later service refresh and fix pack level.
