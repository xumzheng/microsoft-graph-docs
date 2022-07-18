---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ShiftPreferencesRequestBody
{
	AdditionalData = new()
	{
		{"id", "SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7"},
		{"@odata.etag", "1a371e53-f0a6-4327-a1ee-e3c56e4b38aa"},
		{"availability", new List<Object>
		{
		}
	}
};
await graphClient.Users["user-id"].Settings.ShiftPreferences.PutAsync(requestBody);


```