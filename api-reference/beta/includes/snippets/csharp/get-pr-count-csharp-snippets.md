---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Groups["group-id"].Members.User.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Count = true;
	requestConfiguration.QueryParameters.Orderby = new [] { "displayName" };
	requestConfiguration.QueryParameters.Search = "%22displayName:Pr%22";
	requestConfiguration.QueryParameters.Select = new [] { "displayName" , "id" };
	requestConfiguration.Headers.Add("ConsistencyLevel", "eventual");
});


```