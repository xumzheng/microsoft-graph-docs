---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Call
{
	@odata.type = "#microsoft.graph.call",
	CallbackUri = "https://bot.contoso.com/callback",
	Source = new ParticipantInfo
	{
		Identity = new IdentitySet
		{
			@odata.type = "#microsoft.graph.identitySet",
			Application = new Identity
			{
				@odata.type = "#microsoft.graph.identity",
				DisplayName = "Calling Bot",
				Id = "2891555a-92ff-42e6-80fa-6e1300c6b5c6",
			},
		},
		Region = null,
		LanguageId = null,
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
					DisplayName = "John",
					Id = "112f7296-5fa4-42ca-bae8-6a692b15d4b8",
				},
			},
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.invitationParticipantInfo"},
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
		AdditionalData = new()
		{
			{"blob", "<Media Session Configuration>"},
		}
	},
};
var result = await graphClient.Communications.Calls.PostAsync(requestBody);


```