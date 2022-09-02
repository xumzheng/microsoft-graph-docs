---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Security.Cases.EdiscoveryCases.Item.ReviewSets.Item.Queries.Item.ApplyTags.ApplyTagsPostRequestBody
{
	TagsToAdd = new List<Microsoft.Graph.Beta.Models.Security.EdiscoveryReviewTag>
	{
		new EdiscoveryReviewTag
		{
			Id = "d3d99dc704a74801b792b3e1e722aa0d",
		},
	},
};
await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].ReviewSets["ediscoveryReviewSet-id"].Queries["ediscoveryReviewSetQuery-id"].ApplyTags.PostAsync(requestBody);


```