---
title: "Payment requirements for the OneDrive and SharePoint APIs"
description: "This article describes the licensing and payment requirements for the SharePoint and OneDrive APIs in Microsoft Graph."
ms.localizationpriority: high
ms.prod: "files"
ms.custom: scenarios:getting-started
---

# Payment requirements for the OneDrive and SharePoint APIs

This article describes the licensing and payment requirements for the SharePoint and OneDrive APIs in Microsoft Graph.

The following APIs have consumption charges:

- [AssignSensitivityLabel API](http://https://learn.microsoft.com/en-us/graph/api/driveitem-assignsensitivitylabel?view=graph-rest-beta&tabs=http "AssignSensitivityLabel API") [Private Preview] – Asynchronously assigns a sensitivity label to a file hosted in OneDrive or SharePoint online. 

 Note: You must [associate](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory// "associate") or [create](https://docs.microsoft.com/en-us/azure/cost-management-billing/manage/create-subscriptionp:// "create") Azure Subscription for your tenant to call the AssignSensitivityLabel API.  During Private Preview, an Azure billing statement will be created you to see the details of the transactions, however, no charge will be associated with that bill. Please see“Enroll in the Preview" below for instructions on how to apply to be in the Assign Sensitivity Label Private Preview. 

## Licensing model at General Availability 

The AssignSensitivityLabel API, will follow a per call billing model at General Availability. 

## Enroll in the Preview

For your application to enroll in the Preview to call [AssignSensitivityLabel](hhttps://learn.microsoft.com/en-us/graph/api/driveitem-assignsensitivitylabel?view=graph-rest-beta&tabs=httpttp:// "AssignSensitivityLabel"), we require you to complete this request form providing an active Azure subscription. Once we have processed your request form, we will follow up with next steps to onboard your application to billing.

## Frequently asked questions

| Scenario  | Details   |
| ------------ | ------------ |
| What happens if no Azure subscription is provided? | You will see a payment related error 403 Forbidden with error message “Cannot call this API”|
| How do I create an Azure subscription?  |   The Azure subscription must be available in the same tenant where the app is registered. Customers with MCA or EA agreements can get a subscription from their existing account. Is also possible to create a PAYG subscription using a credit card or pay by check or wire transfer, for details see [cost management and billing](https://docs.microsoft.com/en-us/azure/cost-management-billing/microsoft-customer-agreementp:// "cost management and billing").|
| Who is responsible for the payment in the case of multitenant apps? | The organization that owns the app registration.|
| Is it possible to differentiate billing from multitenant or single tenant app? | Yes, tenant information must be provided as part of Azure billing details.  |
| Where can I monitor the cost and billing?  |  A subscription owner, or anyone with appropriate RBAC (Roles Based Access Control) can use Azure Cost Analysis tool to track consumption per day or filter by meter, service name, resource ID among other parameters. For more details refer to our [documentation](https://docs.microsoft.com/en-us/azure/cost-management-billing "documentation"). |
|  Is there a volume discount? | Flat rates apply.   |
|  Are these APIs enrolled in [Microsoft Azure Consumption Commitment (MACC) program](https://docs.microsoft.com/en-us/azure/marketplace/azure-consumption-commitment-enrollment "Microsoft Azure Consumption Commitment (MACC) program")?|  No. |



# See also
[OneDrive file storage API overview](onedrive-concept-overview.md)