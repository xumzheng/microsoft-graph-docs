---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.GroupLifecyclePolicies.MicrosoftGraphRenewGroup.RenewGroupPostRequestBody
{
	GroupId = "ffffffff-ffff-ffff-ffff-ffffffffffff",
};
var result = await graphClient.GroupLifecyclePolicies.MicrosoftGraphRenewGroup.PostAsync(requestBody);


```