---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Participant-idRequestBody
{
	AdditionalData = new()
	{
		{"clientContext", "d45324c1-fcb5-430a-902c-f20af696537c"},
		{"participantMixerLevels", new List<Object>
		{
		}
	}
};
await graphClient.Communications.Calls["call-id"].Participants["participant-id"].PostAsync(requestBody);


```