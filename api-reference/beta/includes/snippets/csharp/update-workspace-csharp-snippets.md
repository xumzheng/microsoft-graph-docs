---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Place
{
	OdataType = "microsoft.graph.workspace",
	AdditionalData = new Dictionary<string, object>
	{
		{
			"nickname" , "Conf Room"
		},
		{
			"building" , "1"
		},
		{
			"label" , "100"
		},
		{
			"capacity" , 50
		},
		{
			"isWheelChairAccessible" , false
		},
	},
};
var result = await graphClient.Places["place-id"].PatchAsync(requestBody);


```