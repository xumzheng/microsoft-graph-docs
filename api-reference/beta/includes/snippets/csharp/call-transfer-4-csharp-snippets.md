---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new TransferPostRequestBody
{
	TransferTarget = new InvitationParticipantInfo
	{
		OdataType = "#microsoft.graph.invitationParticipantInfo",
		EndpointType = EndpointType.Default,
		Identity = new IdentitySet
		{
			OdataType = "#microsoft.graph.identitySet",
			AdditionalData = new Dictionary<string, object>
			{
				{
					"phone" , new 
					{
						OdataType = "#microsoft.graph.identity",
						Id = "+12345678901",
					}
				},
			},
		},
		ReplacesCallId = "e5d39592-99bd-4db8-bca8-30fb894ec51d",
		AdditionalData = new Dictionary<string, object>
		{
			{
				"languageId" , "en-us"
			},
			{
				"region" , "amer"
			},
		},
	},
};
await graphClient.Communications.Calls["call-id"].Transfer.PostAsync(requestBody);


```