---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PlayPromptRequestBody
{
	ClientContext = "d45324c1-fcb5-430a-902c-f20af696537c",
	Prompts = new List<Prompt>
	{
		new Prompt
		{
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.mediaPrompt"},
			}
		},
	}
	Loop = false,
};
var result = await graphClient.Communications.Calls["call-id"].PlayPrompt.PostAsync(requestBody);


```