---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new TimeOff-idRequestBody
{
	AdditionalData = new()
	{
		{"userId", "c5d0c76b-80c4-481c-be50-923cd8d680a1"},
	}
};
await graphClient.Teams["team-id"].Schedule.TimesOff["timeOff-id"].PutAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("Prefer", "return=representation");
});


```