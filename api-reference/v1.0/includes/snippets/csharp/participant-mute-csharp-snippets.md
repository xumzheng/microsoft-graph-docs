---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Communications.Calls.Item.Participants.Item.Mute.MutePostRequestBody
{
	ClientContext = "d45324c1-fcb5-430a-902c-f20af696537c",
};
var result = await graphClient.Communications.Calls["call-id"].Participants["participant-id"].Mute.PostAsync(requestBody);


```