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
			@odata.type = "#microsoft.graph.identitySet",
			User = new Identity
			{
				@odata.type = "#microsoft.graph.identity",
				Id = "550fae72-d251-43ec-868c-373732c2704f",
				DisplayName = "Heidi Steen",
				AdditionalData = new()
				{
					{"tenantId", "72f988bf-86f1-41af-91ab-2d7cd011db47"},
				}
			},
		},
		ReplacesCallId = "e5d39592-99bd-4db8-bca8-30fb894ec51d",
		AdditionalData = new()
		{
			{"@odata.type", "#microsoft.graph.invitationParticipantInfo"},
			{"languageId", "en-us"},
			{"region", "amer"},
		}
	},
};
await graphClient.Communications.Calls["call-id"].Transfer.PostAsync(requestBody);


```