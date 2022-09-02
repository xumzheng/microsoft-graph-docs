---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Me.Calendar.CalendarView.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Startdatetime = "2017-01-01T19:00:00-08:00";
	requestConfiguration.QueryParameters.Enddatetime = "2017-01-07T19:00:00-08:00";
});


```