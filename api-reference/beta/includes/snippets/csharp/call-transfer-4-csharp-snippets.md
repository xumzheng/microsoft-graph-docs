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
			AdditionalData = new()
			{
			}
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