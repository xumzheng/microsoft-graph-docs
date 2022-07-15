---
title: "Introduction to Microsoft Viva Learning"
description: "Learn how to find resources for Microsoft Viva Learning."
ms.localizationpriority: medium
author: "malabikaroy"
ms.prod: "employee-learning"
doc_type: conceptualPageType
---

# Use the Viva Learning API
Viva Learning is a centralized employee learning hub in Microsoft Teams that lets you integrate learning and building skills into your day. In Viva Learning, your team can discover, share, recommend, and learn from content libraries provided by both your organization and partners. They can do all of this without leaving Microsoft Teams.

The Viva Learning APIs in Microsoft Graph enable you to make available your content and learner records (user assignments and completion records) from your Learning Management System (LMS) or learning provider, to Viva Learning. To enable the integration, the following categories of APIs are supported.

- Content APIs for uploading and managing learning content metadata from your LMS or learning provider to Viva Learning.
- Learning record APIs for uploading and managing the assignment and completion records for learners from your LMS or learning provider to Viva Learning.  


## How integrations work?

You can integrate your content and learner records from your Learning Management System (LMS) or learning provider, to Viva Learning by either using out-of-the-box integrations where Viva Learning can pull content metadata and learning records from your LMS or learning provider, or by using the Microsoft Graph APIs where you can push content metadata and learning records from your LMS or learning provider into Viva Learning.

Once the content metadata, learner assignments, and the completion records are uploaded to Viva Learning, they appear in Viva Learning at the following locations:

- The content appears on the home page under *Browse courses* – *Providers* section
- Assignments and completed courses appear on *My Learning* page under *Assigned to you* and *Completed* sections respectively

The Microsoft Graph APIs can be used to  
- Register a provider with Viva Learning, provide a display name, square logo that is displayed on a learning content card, and a long logo that is displayed in the *Details* page which is required for the provider content to show up in Viva Learning. The returned registration ID can be used to make the subsequent calls for content ingestion.
- Enable or disable a registration and update the display name  and logo URLs  for a provider.  
- Retrieve the details about a provider in Viva Learning for a specific **registrationId**.  
- Retrieve the list of registrations in Viva Learning for the provider using the Microsoft Graph API.
- Delete a registration.
- Push content meta data to Viva Learning to make content available within Viva Learning for consumption by users.  
- Read the ingested content by using the **registrationId** of a provider.  
- Retrieve the properties of a learning content object.
- Delete the ingested content.

The following table lists common tasks and the Microsoft Graph APIs that can be used to perform them.

| Task | Http Method |Endpoint |
|:-----|:-----|:-----|
|Register new provider                   | POST   |<https://graph.microsoft.com/beta/employeeExperience/LearningProviders> |
|Update provider registration details    | PATCH  |<https://graph.microsoft.com/beta/employeeExperience/LearningProviders/{id}>  |
|Retrieve provider registration          | GET    |<https://graph.microsoft.com/beta/employeeExperience/LearningProviders/{id}>   |
|Retrieve registrations for all providers| GET    |<https://graph.microsoft.com/beta/employeeExperience/LearningProviders>    |
|Delete or De-register a provider        | DELETE |<https://graph.microsoft.com/beta/employeeExperience/LearningProviders/{id}>    |
|Insert/update learning content| PATCH   |<https://graph.microsoft.com/beta/employeeExperience/learningProviders/{registrationId}/learningContents(externalId=’{externalId}’}>     |
|Retrieve learning content     | GET   |<https://graph.microsoft.com/beta/employeeExperience/learningProviders/{registrationId}/learningContents(externalId=’{externalId}’}>     |
|Delete learning content       | DELETE   |<https://graph.microsoft.com/beta/employeeExperience/learningProviders/{registrationId}/learningContents(externalId=’{externalId}’}>     |
