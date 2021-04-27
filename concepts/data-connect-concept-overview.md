---
title: "Overview of Microsoft Graph Data Connect"
description: "Microsoft Graph Data Connect brings Microsoft 365 data to Microsoft Azure, which gives you access to the best development and hosting tools to work with this data."
author: "ajacks-msft, fercobo-msft"
localization_priority: Priority
ms.prod: "data-connect"
ms.custom: scenarios:getting-started
---

# What is Microsoft Graph Data Connect?

Microsoft Graph Data Connect (MGDC) augments Graph’s transactional model with an intelligent way to access rich data at scale. The data covers how workers communicate, collaborate, manage their time, and go about their workplace duties in your Microsoft 365 tenant. Ideal for big data and machine learning, MGDC allows you to develop applications for analytics, intelligence, and business process optimization by extending M365 data into Azure. By integrating in this way, you will be able to take advantage of Azure’s vast suite of compute, storage, and service catalog options while staying compliant with industry standards and keeping your data secure.

![mgdc-capabilities](images/mgdc-capabilities.png)

Microsoft Graph Data Connect uses Azure Data Factory to copy M365 data to your application’s storage at configurable intervals. It also provides a set of tools to streamline the delivery of this data to Microsoft Azure, letting you access the most applicable development and hosting tools available. MGDC also grants a more granular control and consent model: you can manage data, see who is accessing it, and request specific properties of an entity. This is an improvement to Graph’s traditional model, which either granted or denied applications blanket access to entire entities.

Microsoft Graph Data Connect also lets you enable machine learning scenarios for your organization. In these scenarios, you can create applications that provide valuable information to your stakeholders, train machine learning models, and even perform forecasting based on large amounts of acquired data.
[video placeholder]

## Access to data at scale

Rich applications require access to large amounts of data, often from many users in your organization at once. For this reason, Graph’s standard, transactional data model has a tendency to throttle large datasets. Data delivery requires a complex infrastructure and thousands of API calls, any of which might be throttled due to resource limitations. Microsoft Graph Data Connect resolves this challenge by accessing data in bulk and repeatedly copying M365 data to your application with Azure Data Factory. MGDC also allows you to choose between accessing data from everyone in your organization or just specific groups of people.

## Granular data consent

In the traditional Microsoft Graph consent model, an administrator or user can only grant or deny an application’s request to access specific, predefined sets of entities. For example, a request for Mail.Read includes read access to a fixed set of entities that support Outlook mail, including entire [message](/graph/api/resources/message?view=graph-rest-1.0) instances with all the relevant properties. Microsoft Graph Data Connect enables more granular consent, allowing applications to request access to specific properties in an entity or filter the data in those properties. Administrators must give explicit approval before Microsoft Graph data can be accessed. The request must specify the level of access requested, data policy enforcement, the reason for the request, and the schema of the data requested. As a result, applications can only use data that is essential to their function, and any unrelated content is excluded. For example, an app might consume email metadata but exclude body content and attachments.

## Data security and governance

Microsoft is facilitating rich, connected communication between Microsoft Graph Data Connect and Azure that respects customer data. Microsoft Graph Data Connect supports all Azure-native service capabilities, such as encryption, geo-fencing, auditing, and policy enforcement. In order to minimize compliance management overhead for apps you build with MGDC, you can specify a set of detailed policies that you intend to comply with, which Microsoft 365 administrators can then review. After consent is given for these policies is granted, Microsoft will monitor the application’s adherence to policy. If an application violates (or attempts to violate) a policy established by the organization, Microsoft will stop the flow of data to that application.

## Next steps

To get started, see [Get started with Microsoft Graph Data Connect](data-connect-get-started.md).
