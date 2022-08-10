---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new GetByIdsPostRequestBody
{
	Ids = new List<>
	{
		"84b80893874940a3-97b7-68513b600544",
		"5d6059b6368d-45f8-91e18e07d485f1d0",
	},
	Types = new List<>
	{
		"user",
	},
};
var result = await graphClient.DirectoryObjects.GetByIds.PostAsync(requestBody);


```