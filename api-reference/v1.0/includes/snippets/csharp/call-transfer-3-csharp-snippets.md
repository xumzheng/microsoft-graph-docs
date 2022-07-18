---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new TransferRequestBody
{
	TransferTarget = new InvitationParticipantInfo
	{
		Identity = new IdentitySet
		{
			AdditionalData = new()
			{
			}
		},
		AdditionalData = new()
		{
			{"endpointType", "default"},
			{"languageId", "languageId-value"},
			{"region", "region-value"},
		}
	},
	AdditionalData = new()
	{
		{"clientContext", "9e90d1c1-f61e-43e7-9f75-d420159aae08"},
	}
};
await graphClient.Communications.Calls["call-id"].Transfer.PostAsync(requestBody);


```