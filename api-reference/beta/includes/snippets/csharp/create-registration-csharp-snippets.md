---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new RegistrationRequestBody
{
	AdditionalData = new()
	{
		{"@odata.type", "#microsoft.graph.meetingRegistration"},
		{"subject", "Microsoft Ignite"},
		{"description", "Join us November 2–4, 2021 to explore the latest tools, training sessions, technical expertise, networking opportunities, and more."},
		{"startDateTime", "2021-11-02T08:00:00-08:00"},
		{"endDateTime", "2021-11-04T04:00:00-08:00"},
		{"allowedRegistrant", "everyone"},
		{"speakers", new List<Object>
		{
		}
		{"customQuestions", new List<Object>
		{
		}
	}
};
await graphClient.Me.OnlineMeetings["onlineMeeting-id"].Registration.PostAsync(requestBody);


```