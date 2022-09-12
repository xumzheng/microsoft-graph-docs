---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new User
{
	CustomSecurityAttributes = new CustomSecurityAttributeValue
	{
		AdditionalData = new Dictionary<string, object>
		{
			{
				"Engineering" , new 
				{
					OdataType = "#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
					ProjectDate = "2022-10-01",
				}
			},
		},
	},
};
await graphClient.Users["user-id"].PatchAsync(requestBody);


```