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
			AdditionalData = new()
			{
			}
		},
		CountryCode = null,
		EndpointType = null,
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
				AdditionalData = new()
				{
				}
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
	TenantId = "aa67bd4c-8475-432d-bd41-39f255720e0a",
};
var result = await graphClient.Communications.Calls.PostAsync(requestBody);


```