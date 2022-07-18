---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Contact
{
	GivenName = "Pavel",
	Surname = "Bansky",
	EmailAddresses = new List<Object>
	{
		new 
		{
			AdditionalData = new()
			{
				{"address", "pavelb@contoso.onmicrosoft.com"},
				{"name", "Pavel Bansky"},
				{"type", "personal"},
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
	Phones = new List<Phone>
	{
		new Phone
		{
			Number = "+1 732 555 0102",
			Type = "business",
		},
	}
};
var result = await graphClient.Me.Contacts.PostAsync(requestBody);


```