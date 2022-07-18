---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AdminConsentRequestPolicyRequestBody
{
	AdditionalData = new()
	{
		{"isEnabled", true},
		{"notifyReviewers", true},
		{"remindersEnabled", true},
		{"requestDurationInDays", },
		{"reviewers", new List<Object>
		{
		}
	}
};
await graphClient.Policies.AdminConsentRequestPolicy.PutAsync(requestBody);


```