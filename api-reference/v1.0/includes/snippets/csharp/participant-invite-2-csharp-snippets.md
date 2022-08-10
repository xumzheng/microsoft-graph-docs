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
					"identity" , new 
					{
						OdataType = "#microsoft.graph.identitySet",
						Phone = new 
						{
							OdataType = "#microsoft.graph.identity",
							Id = "+12345678901",
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