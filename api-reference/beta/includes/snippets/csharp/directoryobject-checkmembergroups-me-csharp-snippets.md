---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CheckMemberGroupsPostRequestBody
{
	GroupIds = new List<>
	{
		"fee2c45b-915a-4a64-b130-f4eb9e75525e",
		"4fe90ae7-065a-478b-9400-e0a0e1cbd540",
	},
};
var result = await graphClient.Me.CheckMemberGroups.PostAsync(requestBody);


```