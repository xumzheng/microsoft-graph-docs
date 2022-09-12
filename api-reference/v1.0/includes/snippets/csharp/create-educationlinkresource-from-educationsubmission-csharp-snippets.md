---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EducationSubmissionResource
{
	Resource = new EducationResource
	{
		DisplayName = "Wikipedia",
		OdataType = "#microsoft.graph.educationLinkResource",
		AdditionalData = new Dictionary<string, object>
		{
			{
				"link" , "https://en.wikipedia.org/wiki/Main_Page"
			},
		},
	},
};
var result = await graphClient.Education.Classes["educationClass-id"].Assignments["educationAssignment-id"].Submissions["educationSubmission-id"].Resources.PostAsync(requestBody);


```