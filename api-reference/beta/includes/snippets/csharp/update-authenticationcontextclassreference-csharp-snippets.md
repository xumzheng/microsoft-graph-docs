---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AuthenticationContextClassReference
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"value" , new List<>
			{
				new 
				{
					DisplayName = "Contoso trusted locations",
					Description = "Access is only allowed from trusted locations",
					IsAvailable = true,
				},
			}
		},
	},
};
await graphClient.Identity.ConditionalAccess.AuthenticationContextClassReferences["authenticationContextClassReference-id"].PatchAsync(requestBody);


```