---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PlannerTask
{
	Assignments = new PlannerAssignments
	{
		AdditionalData = new()
		{
		}
	},
	AppliedCategories = new PlannerAppliedCategories
	{
		AdditionalData = new()
		{
			{"category3", true},
			{"category4", false},
		}
	},
};
await graphClient.Planner.Tasks["plannerTask-id"].PatchAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("Prefer", "return=representation");
	requestConfiguration.Headers.Add("If-Match", "W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="");
});


```