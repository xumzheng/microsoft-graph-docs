---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UnifiedGroupSource
{
	IncludedSources = "mailbox, site",
	AdditionalData = new()
	{
		{"group@odata.bind", "https://graph.microsoft.com/v1.0/groups/b96f95c5-b1b3-4142-b039-8ac79e7d2c84"},
	}
};
var result = await graphClient.Compliance.Ediscovery.Cases["case-id"].Custodians["custodian-id"].UnifiedGroupSources.PostAsync(requestBody);


```