---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Me.Events["event-id"].GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Select = new string []{ "subject","start","end","occurrenceId","exceptionOccurrences","cancelledOccurrences" };
	requestConfiguration.QueryParameters.Expand = new string []{ "exceptionOccurrences" };
});


```