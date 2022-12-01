---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new OnlineMeeting
{
	StartDateTime = DateTimeOffset.Parse("2019-07-12T14:30:34.2444915-07:00"),
	EndDateTime = DateTimeOffset.Parse("2019-07-12T15:00:34.2464912-07:00"),
	Subject = "User Token Meeting",
};
var result = await graphClient.Me.OnlineMeetings.PostAsync(requestBody);


```