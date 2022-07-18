---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EducationAssignmentSettings
{
	SubmissionAnimationDisabled = true,
};
await graphClient.Education.Classes["educationClass-id"].AssignmentSettings.PatchAsync(requestBody);


```