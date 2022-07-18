---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Shift-idRequestBody
{
	AdditionalData = new()
	{
		{"id", "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8"},
		{"createdDateTime", "2019-03-14T04:32:51.451Z"},
		{"lastModifiedDateTime", "2019-03-14T05:32:51.451Z"},
		{"userId", "c5d0c76b-80c4-481c-be50-923cd8d680a1"},
		{"schedulingGroupId", "TAG_228940ed-ff84-4e25-b129-1b395cf78be0"},
	}
};
await graphClient.Teams["team-id"].Schedule.Shifts["shift-id"].PutAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("Prefer", "return=representation");
});


```