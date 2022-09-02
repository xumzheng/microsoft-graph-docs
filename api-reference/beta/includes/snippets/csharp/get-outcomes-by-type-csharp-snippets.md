---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Education.Classes["educationClass-id"].Assignments["educationAssignment-id"].Submissions["educationSubmission-id"].Outcomes.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Filter = "isof('microsoft.graph.educationFeedbackResourceOutcome')";
});


```