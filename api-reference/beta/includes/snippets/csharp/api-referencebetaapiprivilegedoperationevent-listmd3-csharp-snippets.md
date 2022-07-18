---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.PrivilegedOperationEvents.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Filter = "(creationDateTime%20ge%202017-06-25T07:00:00Z)%20and%20";
	requestConfiguration.QueryParameters.Count = true;
	requestConfiguration.QueryParameters.Orderby = new [] { "creationDateTime%20desc" };
});


```