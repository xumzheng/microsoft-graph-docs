---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Teams.Item.Schedule.SchedulePutRequestBody
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"enabled" , true
		},
		{
			"timeZone" , "America/Chicago"
		},
		{
			"provisionStatus" , "Completed"
		},
		{
			"provisionStatusCode" , null
		},
		{
			"openShiftsEnabled" , true
		},
		{
			"swapShiftsRequestsEnabled" , true
		},
		{
			"offerShiftRequestsEnabled" , true
		},
		{
			"timeOffRequestsEnabled" , true
		},
		{
			"timeClockEnabled" , true
		},
		{
			"timeClockSettings" , new 
			{
				ApprovedLocation = new 
				{
					Altitude = 1024.13,
					Latitude = 26.13246,
					Longitude = 24.34616,
				},
			}
		},
	},
};
await graphClient.Teams["team-id"].Schedule.PutAsync(requestBody);


```