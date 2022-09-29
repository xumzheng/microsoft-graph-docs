---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new OutlookTask
{
	DueDateTime = new DateTimeTimeZone
	{
		DateTime = "2016-05-06T16:00:00",
		TimeZone = "Eastern Standard Time",
	},
};
var result = await graphClient.Me.Outlook.Tasks["outlookTask-id"].PatchAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("Prefer", "outlook.timezone=\"Eastern Standard Time\"");
});


```