---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Teams["team-id"].Channels["channel-id"].Tabs.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Expand = new [] { "teamsApp" };
	requestConfiguration.QueryParameters.Filter = "teamsApp/id%20eq%20'com.microsoft.teamspace.tab.planner'";
});


```