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
					"identity" , new 
					{
						OdataType = "#microsoft.graph.identitySet",
						User = new 
						{
							OdataType = "#microsoft.graph.identity",
							Id = "278405a3-f568-4b3e-b684-009193463064",
							DisplayName = "string",
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