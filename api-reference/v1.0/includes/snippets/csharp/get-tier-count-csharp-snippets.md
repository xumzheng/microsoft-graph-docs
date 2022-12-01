---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Groups["group-id"].TransitiveMembers.User.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Count = true;
	requestConfiguration.QueryParameters.OrderBy = new string []{ "displayName" };
	requestConfiguration.QueryParameters.Search = "\"displayName:tier\"";
	requestConfiguration.QueryParameters.Select = new string []{ "displayName","id" };
	requestConfiguration.Headers.Add("ConsistencyLevel", "eventual");
});


```