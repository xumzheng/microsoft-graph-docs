---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AnswerRequestBody
{
	CallbackUri = "https://bot.contoso.com/api/calls",
	AcceptedModalities = new List<Modality>
	{
		"audio",
	}
	MediaConfig = new MediaConfig
	{
		@odata.type = "#microsoft.graph.serviceHostedMediaConfig",
		AdditionalData = new()
		{
			{"preFetchMedia", new List<Object>
			{
			}
		}
	},
};
await graphClient.Communications.Calls["call-id"].Answer.PostAsync(requestBody);


```