---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Models.Security.UnifiedGroupSource
{
	Group = new Group
	{
		Mail = "SOCTeam@M365x809305.onmicrosoft.com",
	},
	IncludedSources = Microsoft.Graph.Beta.Models.Security.SourceType.Mailbox | Microsoft.Graph.Beta.Models.Security.SourceType.Site,
};
var result = await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].Custodians["ediscoveryCustodian-id"].UnifiedGroupSources.PostAsync(requestBody);


```