---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.PrivilegedOperationEvents.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Filter = "(creationDateTime ge 2017-06-25T07:00:00Z) and ";
	requestConfiguration.QueryParameters.Count = true;
	requestConfiguration.QueryParameters.Orderby = new string []{ "creationDateTime desc" };
});


```