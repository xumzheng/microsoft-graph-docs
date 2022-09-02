---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SchedulingGroup
{
	DisplayName = "Cashiers",
	IsActive = true,
	UserIds = new List<>
	{
		"c5d0c76b-80c4-481c-be50-923cd8d680a1",
		"2a4296b3-a28a-44ba-bc66-0274b9b95851",
	},
};
var result = await graphClient.Teams["team-id"].Schedule.SchedulingGroups.PostAsync(requestBody);


```