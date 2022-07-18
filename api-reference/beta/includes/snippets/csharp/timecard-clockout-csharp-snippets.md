---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ClockOutRequestBody
{
	Notes = new ItemBody
	{
		ContentType = "text",
		Content = "clock out smaple notes",
	},
	AdditionalData = new()
	{
		{"atAprovedLocation", true},
	}
};
var result = await graphClient.Teams["team-id"].Schedule.TimeCards["timeCard-id"].ClockOut.PostAsync(requestBody);


```