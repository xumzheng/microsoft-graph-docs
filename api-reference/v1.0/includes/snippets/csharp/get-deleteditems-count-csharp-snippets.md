---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Directory.DeletedItems.Group.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Count = true;
	requestConfiguration.QueryParameters.OrderBy = "deletedDateTime%20asc";
	requestConfiguration.QueryParameters.Select = new [] { "id" , "DisplayName" , "deletedDateTime" };
	requestConfiguration.Headers.Add("ConsistencyLevel", "eventual");
});


```