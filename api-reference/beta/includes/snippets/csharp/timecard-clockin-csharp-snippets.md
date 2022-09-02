---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ClockInPostRequestBody
{
	Notes = new ItemBody
	{
		ContentType = BodyType.Text,
		Content = "clock in notes",
	},
	AdditionalData = new Dictionary<string, object>
	{
		{
			"atAprovedLocation" , true
		},
	},
};
var result = await graphClient.Teams["team-id"].Schedule.TimeCards.ClockIn.PostAsync(requestBody);


```