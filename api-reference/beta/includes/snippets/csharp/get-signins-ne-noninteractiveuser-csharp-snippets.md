---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.AuditLogs.SignIns.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Filter = "(signInEventTypes/any)";
	requestConfiguration.QueryParameters.OrderBy = "createdDateTime%20DESC";
	requestConfiguration.QueryParameters.Top = 10;
});


```