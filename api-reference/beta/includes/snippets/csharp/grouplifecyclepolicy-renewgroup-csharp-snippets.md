---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.GroupLifecyclePolicies.RenewGroup.RenewGroupPostRequestBody
{
	GroupId = "ffffffff-ffff-ffff-ffff-ffffffffffff",
};
var result = await graphClient.GroupLifecyclePolicies.RenewGroup.PostAsync(requestBody);


```