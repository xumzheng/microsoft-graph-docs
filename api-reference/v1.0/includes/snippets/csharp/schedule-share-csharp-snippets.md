---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Teams.Item.Schedule.Share.SharePostRequestBody
{
	NotifyTeam = true,
	StartDateTime = DateTimeOffset.Parse("2018-10-08T00:00:00.000Z"),
	EndDateTime = DateTimeOffset.Parse("2018-10-15T00:00:00.000Z"),
};
await graphClient.Teams["team-id"].Schedule.Share.PostAsync(requestBody);


```