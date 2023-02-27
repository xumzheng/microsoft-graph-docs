---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Teams.Item.Schedule.TimeCards.MicrosoftGraphClockIn.ClockInPostRequestBody
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
var result = await graphClient.Teams["team-id"].Schedule.TimeCards.MicrosoftGraphClockIn.PostAsync(requestBody);


```