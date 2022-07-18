---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new InviteRequestBody
{
	Participants = new List<InvitationParticipantInfo>
	{
		new InvitationParticipantInfo
		{
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.invitationParticipantInfo"},
				{"replacesCallId", "a7ebfb2d-871e-419c-87af-27290b22e8db"},
			}
		},
	}
	ClientContext = "f2fa86af-3c51-4bc2-8fc0-475452d9764f",
};
var result = await graphClient.Communications.Calls["call-id"].Participants.Invite.PostAsync(requestBody);


```