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
			User = new Identity
			{
				Id = "550fae72-d251-43ec-868c-373732c2704f",
				DisplayName = "Heidi Steen",
				AdditionalData = new()
				{
					{"tenantId", "72f988bf-86f1-41af-91ab-2d7cd011db47"},
				}
			},
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