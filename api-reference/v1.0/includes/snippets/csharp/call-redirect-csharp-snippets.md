---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new RedirectRequestBody
{
	Targets = new List<InvitationParticipantInfo>
	{
		new InvitationParticipantInfo
		{
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.invitationParticipantInfo"},
			}
		},
	}
	CallbackUri = "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039",
};
await graphClient.Communications.Calls["call-id"].Redirect.PostAsync(requestBody);


```