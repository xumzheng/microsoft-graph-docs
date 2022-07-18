---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new OpenShift-idRequestBody
{
	AdditionalData = new()
	{
		{"schedulingGroupId", "TAG_228940ed-ff84-4e25-b129-1b395cf78be0"},
		{"draftOpenShift", null},
	}
};
await graphClient.Teams["team-id"].Schedule.OpenShifts["openShift-id"].PutAsync(requestBody);


```