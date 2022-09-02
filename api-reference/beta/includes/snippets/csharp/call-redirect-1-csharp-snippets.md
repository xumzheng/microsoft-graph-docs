---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new RedirectPostRequestBody
{
	Targets = new List<InvitationParticipantInfo>
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
						Application = new 
						{
							OdataType = "#microsoft.graph.identity",
							DisplayName = "test bot 2",
							Id = "22bfd41f-550e-477d-8789-f6f7bd2a5e8b",
						},
					}
				},
			},
		},
	},
	CallbackUri = "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039",
};
await graphClient.Communications.Calls["call-id"].Redirect.PostAsync(requestBody);


```