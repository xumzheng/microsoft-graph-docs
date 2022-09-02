---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Directory.DeletedItems.Group.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Count = true;
	requestConfiguration.QueryParameters.Orderby = new string []{ "deletedDateTime asc" };
	requestConfiguration.QueryParameters.Select = new string []{ "id","DisplayName","deletedDateTime" };
	requestConfiguration.Headers.Add("ConsistencyLevel", "eventual");
});


```