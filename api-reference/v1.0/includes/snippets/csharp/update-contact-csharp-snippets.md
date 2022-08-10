---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Contact
{
	HomeAddress = new PhysicalAddress
	{
		Street = "123 Some street",
		City = "Seattle",
		State = "WA",
		PostalCode = "98121",
	},
	Birthday = DateTimeOffset.Parse("1974-07-22"),
};
await graphClient.Me.Contacts["contact-id"].PatchAsync(requestBody);


```