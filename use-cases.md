---

copyright:
  years: 2023
lastupdated: "2024-03-05"

subcollection: zmodernization-fscloud

keywords:

---

{{site.data.keyword.attribute-definition-list}}

# Industry Use Cases
{: #use-cases}

Client use cases are being derived and organized based on industries. The use cases will be described as requirements that would enable clients to derive solutions and make decisions.
{: shortdesc}

## 1. IBM Wazi aaS: Cloud Native development and testing on IBM Cloud for mainframe applications –
{: #dev-test-usecase}

A healthcare client runs mainframe application on IBM Z Systems at their Data Center. Development and Test environments share the MIPS with their staging environment running in the Z System. The client is looking to reduce the MIPS to about 30% so that the cost and maintenance to develop and test these applications will be reduced and as well expedite the business delivery at speed.

z/OS Infrastructure as a Service running on Z Hardware for development and early testing also known as [Wazi as a Service (WaaS)](https://www.ibm.com/cloud/wazi-as-a-service) is a unique service that provides.

- Cloud service with z/OS running on Z LinuxOne hardware which is 8 -15x times faster performance than any z/OS running in emulated x86 hardware.
- On-demand access to a z/OS environment in less than 5 minutes.
- z/OS system that includes the latest and greatest software.
- Automated testing, with security earlier in the development lifecycle.
- Enabling easy deployment of a z/OS system with Wazi Image Builder using standard or custom images.
- Enabling horizontal and vertical scaling on demand based on business needs and pay only for what you use with infrastructure available as a service in a flexible consumption model.
- Deploying an IBM-provided dev and test stock images on the z/OS Virtual Server, or bring a custom image for applications and related components to deploy to the z/OS Virtual Server in VPC.

## 2. Industry Specific Regulations: Modernize with IBM Cloud Framework for Financial Services for regulated industries -
{: #fs-cloud}

A Financial Industry client requires stringent security and compliance rules that are needed to be applied during the build and deployment of custom image data from On-Prem to Development and Test environment. Ensuring the network connectivity in a secure isolated network from public network services is required while building and deploying the custom image from Z systems running at a client’s data center on to IBM Cloud Wazi aaS

The [IBM Cloud Framework for Financial Services](https://cloud.ibm.com/docs/framework-financial-services?topic=framework-financial-services-about) a.k.a IBM FS Cloud is a robust solution designed specifically to cater to the unique needs of regulated institutions, ensuring regulatory compliance, top-notch security, and resiliency both during the initial deployment phase and in ongoing operations. The key components of this framework include.

- a comprehensive set of control requirements, which encompass security and regulatory compliance obligations, as well as cloud best practices.
- best practices involving a shared responsibility model that applies to financial institutions, application providers, and IBM Cloud, ensuring that everyone plays a part in maintaining a secure and compliant environment.

To further facilitate compliance, [reference architectures](https://cloud.ibm.com/docs?tab=solutions&contentType=reference-architecture) are provided to assist in the implementation of control requirements. These architectures can be deployed as infrastructure as code, streamlining the deployment and configuration process. IBM also offers a range of tools and services, such as the IBM Cloud Security and Compliance Center, to empower stakeholders to monitor compliance, address issues, and generate evidence of compliance efficiently.

## 3. Secure Development and Operations DevSecOps: Accelerate DevOps practices with flexible, consumption-based pricing –
{: #devops-usecase}

An insurance client is looking to modernize the applications by refactoring and enhancing the core system to be integrated with new cloud native applications. A process is required to tie into existing source code management like Endevor/RACAF while the developers refactor and move to Git.

IBM Cloud provides deployable architectures with a set of [DevOps Toolchains](https://cloud.ibm.com/docs/ContinuousDelivery?topic=ContinuousDelivery-getting-started&interface=ui) and pipelines. The deployable architecture pipelines use Continuous Integration, Continuous Delivery, Continuous Compliance to meet the industry standards. DevSecOps also leverages popular scanning tools such as SonarQube, GoSec, OWASP Zap (dynamic scan), any unit test framework, and GPG signing. It can also be used with more tools such as external Git providers and artifact stores. DevSecOps supports hybrid deployments, by using private pipeline workers.

## 4. Data Security: Highest Level of Security Encryption with FIPS 140 – Level 4 -

Most regulated industries data used for development and test resides on On-Prem databases and storage. The access to data from the dev and test environment in IBM Cloud should be secured with data security at-rest and in-transit using highest level security services.

[IBM Cloud Hyper Protect Crypto Services](https://www.ibm.com/products/hyper-protect-crypto) is an as-a-service (aaS) key management and encryption solution, which gives you full control over your encryption keys for data protection.

You can enhance your data security by

- Use of the FIPS 140-2 Level 4 hardware security module to leverage the highest security level in the industry.
- Encrypting integrated IBM Cloud Services and applications with Keep Your Own Key (KYOK). Retain complete control of your data encryption keys with technical assurance and provide runtime isolation with confidential computing.
- Enhance your security posture and manage keys with Unified Key Orchestrator in a multicloud environment that includes IBM Cloud, Microsoft Azure, AWS, and Google Cloud Platform
- Protect your sensitive data quantum-safe and stay crypto agile. Currently, Hyper Protect Crypto Services provides quantum safe signing with Dillithium
- Several guidances and regulations around the world, such as from NIST, GDPR, C5, ACSC/ASC, ECUC, ENISA, DPDPA, DORA, and more are met.
