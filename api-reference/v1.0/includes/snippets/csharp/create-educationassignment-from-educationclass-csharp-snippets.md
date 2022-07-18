---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EducationAssignment
{
	DueDateTime = DateTimeOffset.Parse("2021-09-07T00:00:00Z"),
	DisplayName = "Reading test 09.03 #4",
	Instructions = new EducationItemBody
	{
		ContentType = "text",
		Content = "Read chapter 4",
	},
	Grading = new EducationAssignmentGradeType
	{
		@odata.type = "#microsoft.graph.educationAssignmentGradeType",
		AdditionalData = new()
		{
			{"maxPoints", },
		}
	},
	AssignTo = new EducationAssignmentRecipient
	{
		@odata.type = "#microsoft.graph.educationAssignmentGradeType",
	},
	Status = "draft",
	AllowStudentsToAddResourcesToSubmission = true,
};
var result = await graphClient.Education.Classes["educationClass-id"].Assignments.PostAsync(requestBody);


```