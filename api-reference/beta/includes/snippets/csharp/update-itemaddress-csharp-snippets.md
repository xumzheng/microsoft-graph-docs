---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ItemAddress
{
	AllowedAudiences = AllowedAudiences.Me,
	DisplayName = "Secret Hideout",
};
var result = await graphClient.Users["user-id"].Profile.Addresses["itemAddress-id"].PatchAsync(requestBody);


```