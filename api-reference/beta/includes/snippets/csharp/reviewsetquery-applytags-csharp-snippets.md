---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Compliance.Ediscovery.Cases.Item.ReviewSets.Item.Queries.Item.ApplyTags.ApplyTagsPostRequestBody
{
	TagsToAdd = new List<Microsoft.Graph.Beta..Ediscovery.Tag>
	{
		new Tag
		{
			Id = "b4798d14-748d-468e-a1ec-96a2b1d49677",
		},
	},
};
await graphClient.Compliance.Ediscovery.Cases["case-id"].ReviewSets["reviewSet-id"].Queries["reviewSetQuery-id"].ApplyTags.PostAsync(requestBody);


```