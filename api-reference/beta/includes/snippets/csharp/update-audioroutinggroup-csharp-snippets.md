---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AudioRoutingGroup
{
	Id = "oneToOne",
	RoutingMode = RoutingMode.Onetoone,
	Sources = new List<>
	{
		"632899f8-2ea1-4604-8413-27bd2892079f",
	},
	Receivers = new List<>
	{
		"550fae72-d251-43ec-868c-373732c2704f",
		"72f988bf-86f1-41af-91ab-2d7cd011db47",
	},
};
await graphClient.Communications.Calls["call-id"].AudioRoutingGroups["audioRoutingGroup-id"].PatchAsync(requestBody);


```