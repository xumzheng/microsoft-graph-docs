---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SchedulePostRequestBody
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"enabled" , true
		},
		{
			"timeZone" , "America/Chicago"
		},
	},
};
await graphClient.Teams["team-id"].Schedule.PutAsync(requestBody);


```