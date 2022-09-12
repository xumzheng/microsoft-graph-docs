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
		ContentType = BodyType.Text,
		Content = "Read chapter 4",
	},
	Grading = new EducationAssignmentGradeType
	{
		OdataType = "#microsoft.graph.educationAssignmentGradeType",
		AdditionalData = new Dictionary<string, object>
		{
			{
				"maxPoints" , 50
			},
		},
	},
	AssignTo = new EducationAssignmentRecipient
	{
		OdataType = "#microsoft.graph.educationAssignmentGradeType",
	},
	Status = EducationAssignmentStatus.Draft,
	AllowStudentsToAddResourcesToSubmission = true,
};
var result = await graphClient.Education.Classes["educationClass-id"].Assignments.PostAsync(requestBody);


```