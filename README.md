# Google Cloud Platform (GCP) Notes

These notes cover various topics related to using the Google Cloud Platform (GCP) for cloud computing.

## Table of Contents

- [Introduction to Cloud](#introduction-to-cloud)
- [Introduction to GCP](#introduction-to-gcp)
- [Creating a GCP Project](#creating-a-gcp-project)
- [GCP Console](#google-cloud-console)
- [GCP Resources](#google-cloud-resources)
- [GCP Services](#gcp-services)
    - [Identity and Access Management](#identity-and-access-management)
    - [Billing](#billing)
    - [GCP Compute Services](#gcp-compute-services)
        - [Compute Engine](#compute-engine)
        - [Kubernetes Engine](#kubernetes-engine)
- [GCP Cloud Shell](#gcp-cloud-shell)

## Introduction to Cloud

1. Cloud in simple term, is just a set of tool that help you as a developer spend less time managing and more time creating.  
[Being Creative as a developer]
2. Cloud Computing means doing things using other system/computer.  
3. Cloud Computing has three main types
    - Infrastructure As A Service (IAAS)
    - Platform As A Service (PAAS)
    - Software As A Service (SAAS)
4. Google Cloud as a whole consists of many tools, categories into
    - GCP [ IAAS + PAAS ]
    - Gsuit [ SAAS ]

## Introduction to GCP

Google Cloud Platform (GCP) is a collection of cloud computing services that are offered by Google. These services include computing power, storage, and databases, as well as networking, security, and management and monitoring tools. With GCP, you can build and run applications, store and analyze data, and create virtual machines and containers.

## Creating a GCP Project

Before you can start using GCP services, you need to create a GCP project. A project is a container for all the resources you create in GCP. It is used to organize and manage resources, and to control access to them. To create a new project, you can use the [GCP Console](https://console.cloud.google.com/).

## Google Cloud Console

Google cloud console is a powerful graphical (GUI) tool which help to manage Google Cloud resources regardless of their data centre locations.

## Google Cloud Resources

1. GCP resources are fundamentals components that make up google cloud services. Such as
    - Compute engine virtual machine
    - Pub/Sub Topics
    - Cloud Storage Buckets
    - App Engine Instances and so forth...
2. GCP resources are organised hierarchically using projects and folders.
    - **Projects** allow us to group resources together and are the first level of that heirarchy.
    - All resource must belong to exactly one project.
    - Also, projects can belong to organisations, which can further organise company, department, and teams into folders.
    - **Folders** can also contain projects and sub-folders for added flexibility.
3. This heirarchy provides the basis for access control policy inheritance.

## GCP Services

### Identity and Access Management

1. Cloud Identity and Access Management enable us to manage and create access permission for our GCP resources.
2. This service is resource based, which means that it is associated with specific resources like projects, folders, and individual resources such as Compute Engine instances or Cloud Storage buckets.
3. Using Cloud IAM and Admin section we can add users, groups, or service accounts and assign them any # number of roles to grant the permission they need.
4. There are many predefiend roles other than admin and developers.

### Billing

1. GCP Billing is a service that helps manage and track the cost of using GCP resources.
2. The Biling section/service is where we manage **billing account** and link our projects to them.
    - A billing account is essentially a payment payment method (one or more cerdit card information or bank details).
3. A project that does not have a associate billing account or not the billing accounts is not enable, will just not be able to use GCP products beyond their free tiers.
4. In Billing section, we can monitor and control our spending on resources by setting budget alerts to help mange costs.
5. We can also view billing history and usage details.
6. We cna also set up triggered actions for project or accounts as well.
7. We can also generates billing exports as well as reports to better understand our spending.
8. We can also transfer billing ownership to different accounts.

## GCP Compute Services

### Compute Engine

GCP offers a variety of compute services that you can use to run your applications.

[Compute Engine](https://cloud.google.com/compute/) is a service that allows you to create and run virtual machines (VMs) on GCP. With Compute Engine, you can choose from a variety of machine types, operating systems, and disk types, and you can scale your VMs up or down as needed.

### Kubernetes Engine

[Kubernetes Engine](https://cloud.google.com/kubernetes-engine/) is a service that allows you to run and manage containers on GCP. With Kubernetes Engine, you can create and manage clusters of containerized applications, and you can scale your clusters up or down as needed.

## GCP Cloud Shell

1. Google cloud shell provides us with command line access (CLI) to GCP resources directly from browser without having the need to install anything.
2. Google cloud shell is accessible from the browser in cloud console and is powered by a small virtual machine with persistdent disk space and up-to-date software for all the development needs.
