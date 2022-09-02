---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta..Security.UserSource
{
	Email = "admin@M365x809305.onmicrosoft.com",
	IncludedSources = SourceType.Mailbox, site,
};
var result = await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].LegalHolds["ediscoveryHoldPolicy-id"].UserSources.PostAsync(requestBody);


```