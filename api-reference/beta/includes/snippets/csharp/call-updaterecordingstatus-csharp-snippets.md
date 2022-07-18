---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UpdateRecordingStatusRequestBody
{
	ClientContext = "clientContext-value",
	Status = "notRecording | recording | failed",
};
var result = await graphClient.Communications.Calls["call-id"].UpdateRecordingStatus.PostAsync(requestBody);


```