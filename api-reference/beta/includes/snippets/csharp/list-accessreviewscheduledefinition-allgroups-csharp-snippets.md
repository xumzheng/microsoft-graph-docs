---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.IdentityGovernance.AccessReviews.Definitions.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Filter = "contains(scope/microsoft.graph.accessReviewQueryScope/query,%20'./members')";
});


```