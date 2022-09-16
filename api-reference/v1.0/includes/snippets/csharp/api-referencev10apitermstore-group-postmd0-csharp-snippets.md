---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Models.TermStore.Group
{
	DisplayName = "myGroup",
};
var result = await graphClient.Sites["site-id"].TermStore.Groups.PostAsync(requestBody);


```