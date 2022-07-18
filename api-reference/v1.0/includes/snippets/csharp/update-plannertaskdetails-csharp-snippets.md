---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PlannerTaskDetails
{
	PreviewType = "noPreview",
	References = new PlannerExternalReferences
	{
		AdditionalData = new()
		{
			{"http%3A//www%2Ebing%2Ecom", null},
		}
	},
	Checklist = new PlannerChecklistItems
	{
		AdditionalData = new()
		{
			{"a93c93c5-10a6-4167-9551-8bafa09967a7", null},
		}
	},
};
await graphClient.Planner.Tasks["plannerTask-id"].Details.PatchAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("Prefer", "return=representation");
	requestConfiguration.Headers.Add("If-Match", "W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="");
});


```