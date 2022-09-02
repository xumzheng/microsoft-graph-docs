---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new TimeOffReason
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"displayName" , "Vacation"
		},
		{
			"iconType" , "plane"
		},
		{
			"isActive" , true
		},
	},
};
await graphClient.Teams["team-id"].Schedule.TimeOffReasons["timeOffReason-id"].PutAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("Prefer", "return=representation");
});


```