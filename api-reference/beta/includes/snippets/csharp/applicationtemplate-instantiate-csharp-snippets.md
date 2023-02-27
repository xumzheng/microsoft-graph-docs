---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.ApplicationTemplates.Item.MicrosoftGraphInstantiate.InstantiatePostRequestBody
{
	DisplayName = "testProperties",
};
var result = await graphClient.ApplicationTemplates["applicationTemplate-id"].MicrosoftGraphInstantiate.PostAsync(requestBody);


```