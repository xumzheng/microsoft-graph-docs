---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Communications.Calls.Item.Answer.AnswerPostRequestBody
{
	CallbackUri = "callbackUri-value",
	MediaConfig = new MediaConfig
	{
		OdataType = "#microsoft.graph.appHostedMediaConfig",
		AdditionalData = new Dictionary<string, object>
		{
			{
				"blob" , "<Media Session Configuration Blob>"
			},
		},
	},
	AcceptedModalities = new List<Modality?>
	{
		Modality.Audio,
	},
	ParticipantCapacity = 200,
};
await graphClient.Communications.Calls["call-id"].Answer.PostAsync(requestBody);


```