---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PlannerUser
{
	FavoritePlanReferences = new PlannerFavoritePlanReferenceCollection
	{
		AdditionalData = new()
		{
			{"7oTB5aMIAE2rVo-1N-L7RmQAGX2q", null},
		}
	},
	RecentPlanReferences = new PlannerRecentPlanReferenceCollection
	{
		AdditionalData = new()
		{
		}
	},
};
await graphClient.Me.Planner.PatchAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("Prefer", "return=representation");
	requestConfiguration.Headers.Add("If-Match", "W/"JzEtVXNlckRldGFpbHMgQEBAQEBAQEBAQEBAQEBIWCc="");
});


```