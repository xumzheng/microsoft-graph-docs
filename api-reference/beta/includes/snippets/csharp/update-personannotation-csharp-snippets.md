---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PersonAnnotation
{
	AllowedAudiences = AllowedAudiences.Organization,
};
await graphClient.Users["user-id"].Profile.Notes["personAnnotation-id"].PatchAsync(requestBody);


```