---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new InvitePostRequestBody
{
	Participants = new List<InvitationParticipantInfo>
	{
		new InvitationParticipantInfo
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"@odata.type" , "#microsoft.graph.invitationParticipantInfo"
				},
				{
					"replacesCallId" , "a7ebfb2d-871e-419c-87af-27290b22e8db"
				},
				{
					"participantId" , "7d501bf1-5ee4-4605-ba92-0ae4513c611c"
				},
				{
					"identity" , new 
					{
						OdataType = "#microsoft.graph.identitySet",
						User = new 
						{
							OdataType = "#microsoft.graph.identity",
							Id = "682b6c37-0729-4fab-ace6-d730d5d9137e",
							IdentityProvider = "AAD",
						},
					}
				},
			},
		},
	},
	ClientContext = "f2fa86af-3c51-4bc2-8fc0-475452d9764f",
};
var result = await graphClient.Communications.Calls["call-id"].Participants.Invite.PostAsync(requestBody);


```