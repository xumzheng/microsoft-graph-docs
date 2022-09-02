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
	Sources = new List<string>
	{
		"632899f8-2ea1-4604-8413-27bd2892079f",
	},
	Receivers = new List<string>
	{
		"550fae72-d251-43ec-868c-373732c2704f",
	},
};
var result = await graphClient.Communications.Calls["call-id"].AudioRoutingGroups.PostAsync(requestBody);


```