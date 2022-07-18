---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Identity.ConditionalAccess.Policies.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Filter = "displayName%20eq%20'SimplePolicy1'%20or%20displayName%20eq%20'SimplePolicy2'";
});


```