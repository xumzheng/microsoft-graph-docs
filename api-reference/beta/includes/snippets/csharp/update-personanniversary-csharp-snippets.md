---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PersonAnnualEvent
{
	AllowedAudiences = AllowedAudiences.Contacts,
};
var result = await graphClient.Me.Profile.Anniversaries["personAnnualEvent-id"].PatchAsync(requestBody);


```