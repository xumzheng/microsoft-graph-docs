---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Groups.Item.MicrosoftGraphEvaluateDynamicMembership.EvaluateDynamicMembershipPostRequestBody
{
	MemberId = "319b41e8-d9e4-42f8-bdc9-741113f48b33",
};
var result = await graphClient.Groups["group-id"].MicrosoftGraphEvaluateDynamicMembership.PostAsync(requestBody);


```