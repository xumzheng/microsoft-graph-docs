---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Me.CalendarView.Delta().GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Skiptoken = "R0usmcCM996atia_s";
	requestConfiguration.Headers.Add("Prefer", "odata.maxpagesize=2");
});


```