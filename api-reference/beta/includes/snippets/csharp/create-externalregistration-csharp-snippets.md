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
		{"@odata.type", "#microsoft.graph.externalMeetingRegistration"},
		{"allowedRegistrant", "everyone"},
	}
};
await graphClient.Me.OnlineMeetings["onlineMeeting-id"].Registration.PostAsync(requestBody);


```