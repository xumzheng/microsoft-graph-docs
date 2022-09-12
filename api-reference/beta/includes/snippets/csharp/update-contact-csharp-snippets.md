---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Contact
{
	EmailAddresses = new List<TypedEmailAddress>
	{
		new TypedEmailAddress
		{
			Type = EmailType.Personal,
			Name = "Pavel Bansky",
			Address = "pavelb@adatum.onmicrosoft.com",
		},
		new TypedEmailAddress
		{
			Address = "pavelb@fabrikam.onmicrosoft.com",
			Name = "Pavel Bansky",
			Type = EmailType.Other,
			OtherLabel = "Volunteer work",
		},
	},
};
await graphClient.Me.Contacts["contact-id"].PatchAsync(requestBody);


```