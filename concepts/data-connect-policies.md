---
title: "Microsoft Graph Data Connect policies and billing"
description: "Learn about Azure policies supported for an app built with Microsoft 365 data and the bill associated with the Azure Synapse or Azure Data Factory you are using."
author: "rimisra2"
ms.localizationpriority: high
ms.prod: "data-connect"
---

# Microsoft Graph Data Connect policies and billing

Microsoft Graph Data Connect uses [Azure managed applications](/azure/managed-applications/overview) to allow you to create and deploy your solutions in your Azure environment. Managed applications let you support certain Azure policies, giving customers greater confidence and comfortability when using your applications.

## Policies

The following Azure policies are supported for an Azure managed application built by using Microsoft 365 data:

- [Azure Policy built-in definitions for Azure Storage](/azure/storage/common/policy-reference)
- [Introduction to Azure Data Lake Storage Gen2](/azure/storage/blobs/data-lake-storage-introduction)
- [Azure Policy built-in definitions for Azure Data Lake Storage Gen1](/azure/data-lake-store/policy-reference)

> [!NOTE]
> Azure Data Lake Storage Gen1 and Gen2 use different policies because Azure Data Lake Storage Gen2 implements Azure Storage.

When you select any of the policies during Azure Marketplace publishing, the policy compliance status is checked and enforced for all installations of your application. All selected policies that are compliant are shown to the data approvers as part of the data request. Any policy compliance violation causes the pipeline run to fail and stop the data extraction.

## Billing

A bill is associated with the Azure subscription of the Azure Synapse or Azure Data Factory you are using. The price in this new billing model is based on the number of Microsoft Graph objects that you are accessing. For more information about billing, see the [Pricing page](https://azure.microsoft.com/pricing/details/graph-data-connect/).

Microsoft Graph Data Connect consumption charges are billed monthly on a pay-as-you-go basis. The Data Connect billing unit is in a multiple of 1000s of objects, where 1 object maps to 1 individual instance of an entity in Microsoft 365. For example, 1 email == 1 object, 1 file == 1 object, 1 Teams chat message == 1 object, and so on. 

We have some datasets available for free or are currently free in preview while other datasets are charged. Microsoft Graph Data Connect offers datasets across multiple different Microsoft 365 products and services. For more information on datasets that are available through Microsoft Graph Data Connect, please refer to [Dataset, regions and sinks](/concepts/data-connect-datasets.md#datasets).

There is no charge for extraction of objects from the following datasets:
- BasicDataSet_v0.User_v0
- BasicDataSet_v0.User_v1
- BasicDataSet_v0.MailboxSettings
- BasicDataSet_v0.Manager
- BasicDataSet_v0.DirectReport
- BasicDataSet_v0.GroupDetails
- BasicDataSet_v0.GroupMembers
- BasicDataSet_v0.GroupOwners

## Estimating copy speed
Extracting all the data from your Microsoft 365 tenant to Azure can take time. The total time a copy takes depends on the number of records to be extracted. This number can vary between tenants of the same data range. If the number of records is known, it is possible to estimate the time it will take to extract most of them. The total time for one extraction job can still be higher as even if one user is not extracted, the extraction will continue until all data is extracted or the deadline of 24 hours is met. 

Based on some assumptions, the following example represents one possible calculation.

Total records per user for 60 days: 30000 (assuming 500 records are created for this user per day).
- Expected extraction time for 3000 users: 2hr bootstrap/clean up time + (30000/100) min + 2hr buffer time = 2hr + 5hr + 2hr = 9hr
- Expected extraction time for 6000 users: 2hr bootstrap/clean up time + (30000/100)*2 min + 2hr buffer time = 2hr + 10hr + 2hr = 14hr
- Expected extraction time for 12000 users: 2hr bootstrap/clean up time + (30000/100)*4 min + 2hr buffer time = 2hr + 20hr + 2hr = 24hr

Based on above assumption on number of records, it is possible to extract up to 12000 users in a day for the last 60 days worth of data (where each day has around 500 records).

> **Note:** It's not recommended to extract too many datasets for same users and bulk extractions simultaneously.

## See also

- [User selection and filtering](data-connect-filtering.md)
- [Data Connect frequently asked questions](data-connect-faq.md)
- [Dataset, regions and sinks](/concepts/data-connect-datasets.md#datasets).
