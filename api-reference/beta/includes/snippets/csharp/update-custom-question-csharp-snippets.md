---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new MeetingRegistrationQuestion
{
	AnswerInputType = AnswerInputType.Radiobutton,
	AnswerOptions = new List<string>
	{
		"Software Engineer",
		"Software Development Manager",
		"Product Manager",
		"Data scientist",
		"Other",
	},
};
await graphClient.Me.OnlineMeetings["onlineMeeting-id"].Registration.CustomQuestions["meetingRegistrationQuestion-id"].PatchAsync(requestBody);


```