---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new RecordResponseRequestBody
{
	BargeInAllowed = true,
	ClientContext = "d45324c1-fcb5-430a-902c-f20af696537c",
	Prompts = new List<Prompt>
	{
		new Prompt
		{
			@odata.type = "#microsoft.graph.mediaPrompt",
			AdditionalData = new()
			{
			}
		},
	}
	MaxRecordDurationInSeconds = 10,
	InitialSilenceTimeoutInSeconds = 5,
	MaxSilenceTimeoutInSeconds = 2,
	PlayBeep = true,
	StopTones = new List<String>
	{
		"#",
		"1",
		"*",
	}
};
var result = await graphClient.Communications.Calls["call-id"].RecordResponse.PostAsync(requestBody);


```