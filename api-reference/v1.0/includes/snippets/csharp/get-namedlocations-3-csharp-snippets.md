---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Identity.ConditionalAccess.NamedLocations.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Filter = "createdDateTime ge 2019-09-01T00:00:00Z";
});


```