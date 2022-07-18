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
			@odata.type = "#microsoft.graph.identitySet",
			User = new Identity
			{
				@odata.type = "#microsoft.graph.identity",
				Id = "550fae72-d251-43ec-868c-373732c2704f",
				DisplayName = "Heidi Steen",
			},
		},
		ReplacesCallId = "e5d39592-99bd-4db8-bca8-30fb894ec51d",
		AdditionalData = new()
		{
			{"@odata.type", "#microsoft.graph.invitationParticipantInfo"},
			{"endpointType", "default"},
		}
	},
};
await graphClient.Communications.Calls["call-id"].Transfer.PostAsync(requestBody);


```