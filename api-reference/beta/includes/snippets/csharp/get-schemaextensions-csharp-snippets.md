---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.SchemaExtensions.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Filter = "id%20eq%20'graphlearn_test'";
});


```