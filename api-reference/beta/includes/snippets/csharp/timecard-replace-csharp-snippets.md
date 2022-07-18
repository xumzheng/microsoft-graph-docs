---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new TimeCard-idRequestBody
{
	AdditionalData = new()
	{
		{"userId", "70e47528-2fae-42b5-9d8e-ee73ccd90603"},
		{"state", "clockedOut"},
		{"confirmedBy", "None"},
		{"notes", null},
		{"breaks", new List<Object>
		{
		}
	}
};
await graphClient.Teams["team-id"].Schedule.TimeCards["timeCard-id"].PutAsync(requestBody);


```