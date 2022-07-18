---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EducationOutcome
{
	@odata.type = "#microsoft.graph.educationRubricOutcome",
	AdditionalData = new()
	{
		{"rubricQualityFeedback", new List<Object>
		{
		}
		{"rubricQualitySelectedLevels", new List<Object>
		{
		}
	}
};
await graphClient.Education.Classes["educationClass-id"].Assignments["educationAssignment-id"].Submissions["educationSubmission-id"].Outcomes["educationOutcome-id"].PatchAsync(requestBody);


```