---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Teams.Item.Schedule.TimeCards.Item.MicrosoftGraphClockOut.ClockOutPostRequestBody
{
	Notes = new ItemBody
	{
		ContentType = BodyType.Text,
		Content = "clock out smaple notes",
	},
	AdditionalData = new Dictionary<string, object>
	{
		{
			"atAprovedLocation" , true
		},
	},
};
var result = await graphClient.Teams["team-id"].Schedule.TimeCards["timeCard-id"].MicrosoftGraphClockOut.PostAsync(requestBody);


```