---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new LinkedResource_v2
{
	WebUrl = "https://microsoft.com",
	ApplicationName = "Microsoft",
	DisplayName = "Microsoft Web page",
	ExternalId = "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9",
};
var result = await graphClient.Me.Tasks.Lists["baseTaskList-id"].Tasks["baseTask-id"].LinkedResources["linkedResource_v2-id"].PatchAsync(requestBody);


```