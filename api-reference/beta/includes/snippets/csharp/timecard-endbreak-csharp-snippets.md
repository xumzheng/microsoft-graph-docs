---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Teams.Item.Schedule.TimeCards.Item.MicrosoftGraphEndBreak.EndBreakPostRequestBody
{
	Notes = new ItemBody
	{
		ContentType = BodyType.Text,
		Content = "end break smaple notes",
	},
	AdditionalData = new Dictionary<string, object>
	{
		{
			"atAprovedLocation" , true
		},
	},
};
var result = await graphClient.Teams["team-id"].Schedule.TimeCards["timeCard-id"].MicrosoftGraphEndBreak.PostAsync(requestBody);


```