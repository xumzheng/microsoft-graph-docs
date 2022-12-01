---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Communications.Calls.Item.UpdateRecordingStatus.UpdateRecordingStatusPostRequestBody
{
	ClientContext = "clientContext-value",
	Status = RecordingStatus.NotRecording | RecordingStatus.Recording | RecordingStatus.Failed,
};
var result = await graphClient.Communications.Calls["call-id"].UpdateRecordingStatus.PostAsync(requestBody);


```