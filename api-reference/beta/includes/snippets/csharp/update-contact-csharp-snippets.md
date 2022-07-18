---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Contact
{
	EmailAddresses = new List<Object>
	{
		new 
		{
			AdditionalData = new()
			{
				{"type", "personal"},
				{"name", "Pavel Bansky"},
				{"address", "pavelb@adatum.onmicrosoft.com"},
			}
		},
		new 
		{
			AdditionalData = new()
			{
				{"address", "pavelb@fabrikam.onmicrosoft.com"},
				{"name", "Pavel Bansky"},
				{"type", "other"},
				{"otherLabel", "Volunteer work"},
			}
		},
	}
};
await graphClient.Me.Contacts["contact-id"].PatchAsync(requestBody);


```