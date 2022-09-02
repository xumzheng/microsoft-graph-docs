---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Groups["group-id"].CalendarView.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Startdatetime = "2017-01-01T19:00:00-08:00";
	requestConfiguration.QueryParameters.Enddatetime = "2017-10-01T19:00:00.00-08:00";
	requestConfiguration.Headers.Add("Prefer", "outlook.body-content-type=\"text\"");
});


```