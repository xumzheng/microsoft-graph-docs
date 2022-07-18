---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AnswerRequestBody
{
	CallbackUri = "callbackUri-value",
	MediaConfig = new MediaConfig
	{
		@odata.type = "#microsoft.graph.appHostedMediaConfig",
		AdditionalData = new()
		{
			{"blob", "<Media Session Configuration Blob>"},
		}
	},
	AcceptedModalities = new List<Modality>
	{
		"audio",
	}
	ParticipantCapacity = 200,
};
await graphClient.Communications.Calls["call-id"].Answer.PostAsync(requestBody);


```