+++
date= "2016-03-08T21:07:13+01:00"
title= "AZ-203"
type= "index"
weight= 0
+++

# Introduction
This site provides guidance in studing for the microsoft exam AZ-203

The exam can be placed at your own home from monday to saturday from 6:45 am to 12:00 local hour amazing.

## Links
+ [Guidance](https://www.isaaclevin.com/post/az-203-study-guide/)
+ [Azure free tier](https://azure.microsoft.com/en-us/free/?ref=portal)


## Exam summary

### Develop Azure Infraestructer as a service (IaaS). computes a 10-15%

 + Implement solutions that use virtual machines (VM)
   + Provision VMs
   + Create ARM templates
   + Configure Azure Disk Encryption for VMs
 + Implements batch jobs by using Azure Batch Services
   + Manage batch jobs by using Batch Service API
   + Run a batch job by using Azure CLI, Azure portal, and other tools (.NET, python)
   + Write code to run an azure batch services batch job
 + Create containerized solutions
   + Create an azure Managed Kubertness service (AKS) cluster
   + Create container images for solutions
   + Publish an image to the Azure Container Registry.
   + Run containers by using Azure Container Instance or AKS (ACI, AKS)

### Develop Azure platform as a service (PaaS). computes a 20-25%

+ Create Azure App Service Web Apps
  + Create and Azure App Service Web App (.NET with others in TOC)
  + Create an Azure App Service background task by using Webjobs (Create WebJobs)
  + Enable diagnogtics logging (Azure App Service diagnogtics overview)
+ Create Azure App Service Mobile apps
  + Add push notifications for mobile apps.
  + Enable offline sync for mobile app.
  + Implement a remote instrumentation strategy for mobile devices (Use Teamviewer to remotely administer intune devices)
+ Create Azure App Service API apps
  + Create an Azure App Service API app 
  + Create documentation for  the API by using open source and other tools
+ Implement Azure functions
  + Implement input and output bindings for a function
  + Implement function triggers by using data operations, timers and webhooks
  + Implement Azure Durable Functions
  + Create Azure Function apps by using Visual Studio.

### Develop for azure storage. computes a 15-20%

+ Develop solutions that use storage tables
  + Design and implemnt policies for tables
  + Query table storage by using code
  + Implement partitioning schemes
+ Develop solutions that use Cosmos DB storage
  + CRUD by using appropriate APIs
  + Implement partitioning schemes
  + Set the appropiate consistency level for operations
+ Develop solutions that use a relational database
  + Provision and configure relational databases
  + Configure elastic pools for Azure SQL Database
  + CRUD by using code
+ Develop solutions that use blob storage
  + Move items in Blob storage between storage accounts or containers (c# Code, AzCopy)
  + Set and retrieve properties and metadata
  + Implement blob leasing
  + Implement data archiving and retention

### Implement Azure Security. computes a 10-15%

+ Implement authentication
  + Implement authentication by using certificates, form-based or tokens
  + Implement multi-factor or windows authentication by using Azure AD
  + Implement OAuth2 authentication
  + Implement Managed Service Identity (MSI) / service Principal authorization
+ Implement access control
  + Implement CBAC (Claims-Based Access Control) Authorization
  + Implement RBAC (Role Based Access Control)
  + Create shared access signatures
+ Implement Secure data solutions
  + Encrypt and decrypt data at rest and in transit
  + Create, read, update, and delete keys, secrets and certificates by using the keyvault API

### Monitor, Troubleshoot and optimize Azure solutions. computes a 15-20%

+ Develop code to support scalability of apps and services.
  + Implement autoscaling rules and patterns.
  + Implement code that handles transient faults.
+ Integrate caching and content delivery within solutions.
  + Storage and retrieve data in Azure Redis cache
  + Develop code to implement CDN's in solutions
  + Invalidate cache content CDn or Redis
+ Instrument solutions to support monitoring and logging
  + Configure instrumentation in an app or service by using application insights
  + Analyze and troubleshoot solutions by using Azure monitor
  + Implement Application Insights Web Test and alerts

### Connect to and Consume Azure Services and Third-party Services. computes a 20-25%

+ Develop an app service logic app
  + Create a Logic App
  + Create a custom connector for logic apps
  + Create a custom template for logic apps
+ Integrate Azure Search within solutions
  + Create an Azure Search index
  + Import searchable data
  + Query the Azure Search index
+ Establish API Gateways
  + Create an APIM instance
  + Configure authentication for APIS
  + Define policies for APIs
+ Develop event-based solutions
  + Implement solutions that use Azure Event Grid
  + Implement solutions that use Azure Notification Hubs
  + Implement solutions that use Azure Event Hubs
+ Develop message-based solutions
  + Implement solutions that use Azure Service Bus
  + Implement solutions that use Azure Queue Storage queues