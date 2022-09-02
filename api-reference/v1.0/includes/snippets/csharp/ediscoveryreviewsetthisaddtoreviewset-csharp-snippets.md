---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Security.Cases.EdiscoveryCases.Item.ReviewSets.Item.AddToReviewSet.AddToReviewSetPostRequestBody
{
	Search = new Search
	{
		Id = "c17e91d6-6bc0-4ecb-b388-269ea3d4ffb7",
	},
	AdditionalDataOptions = Microsoft.Graph.Models.Security.AdditionalDataOptions.LinkedFiles,
};
await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].ReviewSets["ediscoveryReviewSet-id"].AddToReviewSet.PostAsync(requestBody);


```