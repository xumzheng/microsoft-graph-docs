---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

await graphClient.Users["user-id"].OnlineMeetings["onlineMeeting-id"].Transcripts["callTranscript-id"].Content.GetAsync((requestConfiguration) =>
{
	requestConfiguration.Headers.Add("Accept", "application/vnd.openxmlformats-officedocument.wordprocessingml.document");
});


```