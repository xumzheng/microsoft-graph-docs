---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EdiscoveryHoldPolicy
{
	Displayname = "My legalHold with sources",
	Description = "Created from Graph API",
	ContentQuery = "Bazooka",
	AdditionalData = new()
	{
		{"userSources@odata.bind", new List<Object>
		{
		}
		{"siteSources@odata.bind", new List<Object>
		{
		}
	}
};
var result = await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].LegalHolds.PostAsync(requestBody);


```