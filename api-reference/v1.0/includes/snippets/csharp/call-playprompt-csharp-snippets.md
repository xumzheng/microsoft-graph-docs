---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PlayPromptPostRequestBody
{
	ClientContext = "d45324c1-fcb5-430a-902c-f20af696537c",
	Prompts = new List<Prompt>
	{
		new Prompt
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"@odata.type" , "#microsoft.graph.mediaPrompt"
				},
				{
					"mediaInfo" , new 
					{
						OdataType = "#microsoft.graph.mediaInfo",
						Uri = "https://cdn.contoso.com/beep.wav",
						ResourceId = "1D6DE2D4-CD51-4309-8DAA-70768651088E",
					}
				},
			},
		},
	},
};
var result = await graphClient.Communications.Calls["call-id"].PlayPrompt.PostAsync(requestBody);


```