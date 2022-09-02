---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.AppCatalogs.TeamsApps.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Filter = "externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'";
});


```