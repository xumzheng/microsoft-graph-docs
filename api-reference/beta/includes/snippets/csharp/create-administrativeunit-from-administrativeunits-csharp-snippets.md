---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AdministrativeUnit
{
	DisplayName = "Seattle District Technical Schools",
	Description = "Seattle district technical schools administration",
	AdditionalData = new Dictionary<string, object>
	{
		{
			"membershipType" , "Dynamic"
		},
		{
			"membershipRule" , "(user.country -eq \"United States\")"
		},
		{
			"membershipRuleProcessingState" , "On"
		},
	},
};
var result = await graphClient.AdministrativeUnits.PostAsync(requestBody);


```