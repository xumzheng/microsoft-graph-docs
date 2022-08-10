---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EducationAssignmentDefaults
{
	AddedStudentAction = EducationAddedStudentAction.Assignifopen,
	AddToCalendarAction = EducationAddToCalendarOptions.Studentsandteamowners,
	NotificationChannelUrl = "https://graph.microsoft.com/beta/teams('id')/channels('id')",
};
await graphClient.Education.Classes["educationClass-id"].AssignmentDefaults.PatchAsync(requestBody);


```