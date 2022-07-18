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
		EndpointType = "default",
		Identity = new IdentitySet
		{
			AdditionalData = new()
			{
			}
		},
		AdditionalData = new()
		{
			{"languageId", "languageId-value"},
			{"region", "region-value"},
		}
	},
};
await graphClient.Communications.Calls["call-id"].Transfer.PostAsync(requestBody);


```