---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Call
{
	@odata.type = "#microsoft.graph.call",
	Direction = "outgoing",
	Subject = "Create a group call with app hosted media",
	CallbackUri = "https://bot.contoso.com/callback",
	Source = new ParticipantInfo
	{
		Identity = new IdentitySet
		{
			@odata.type = "#microsoft.graph.identitySet",
			Application = new Identity
			{
				@odata.type = "#microsoft.graph.identity",
				DisplayName = "TestBot",
				Id = "dd3885da-f9ab-486b-bfae-85de3d445555",
			},
		},
		AdditionalData = new()
		{
			{"@odata.type", "#microsoft.graph.participantInfo"},
		}
	},
	Targets = new List<InvitationParticipantInfo>
	{
		new InvitationParticipantInfo
		{
			Identity = new IdentitySet
			{
				@odata.type = "#microsoft.graph.identitySet",
				User = new Identity
				{
					@odata.type = "#microsoft.graph.identity",
					DisplayName = "user1",
					Id = "98da8a1a-1b87-452c-a713-65d3f10b5555",
				},
			},
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.invitationParticipantInfo"},
			}
		},
		new InvitationParticipantInfo
		{
			Identity = new IdentitySet
			{
				@odata.type = "#microsoft.graph.identitySet",
				User = new Identity
				{
					@odata.type = "#microsoft.graph.identity",
					DisplayName = "user2",
					Id = "bf5aae9a-d11d-47a8-93b1-782504c95555",
				},
			},
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.participantInfo"},
			}
		},
	}
	RequestedModalities = new List<Modality>
	{
		"audio",
	}
	MediaConfig = new MediaConfig
	{
		@odata.type = "#microsoft.graph.appHostedMediaConfig",
		RemoveFromDefaultAudioGroup = false,
		AdditionalData = new()
		{
			{"blob", "<Media Session Configuration>"},
		}
	},
	TenantId = "aa67bd4c-8475-432d-bd41-39f255720e0a",
};
var result = await graphClient.Communications.Calls.PostAsync(requestBody);


```