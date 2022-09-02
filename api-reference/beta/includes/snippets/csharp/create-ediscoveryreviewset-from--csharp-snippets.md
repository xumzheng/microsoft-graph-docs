---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta..Security.EdiscoveryReviewSet
{
	DisplayName = "My review set 2",
};
var result = await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].ReviewSets.PostAsync(requestBody);


```