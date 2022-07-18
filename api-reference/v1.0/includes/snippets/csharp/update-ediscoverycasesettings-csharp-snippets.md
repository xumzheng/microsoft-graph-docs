---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EdiscoveryCaseSettings
{
	@odata.type = "#microsoft.graph.security.ediscoveryCaseSettings",
	RedundancyDetection = new RedundancyDetectionSettings
	{
		AdditionalData = new()
		{
			{"@odata.type", "microsoft.graph.security.redundancyDetectionSettings"},
		}
	},
	TopicModeling = new TopicModelingSettings
	{
		AdditionalData = new()
		{
			{"@odata.type", "microsoft.graph.security.topicModelingSettings"},
		}
	},
	Ocr = new OcrSettings
	{
		AdditionalData = new()
		{
			{"@odata.type", "microsoft.graph.security.ocrSettings"},
		}
	},
};
await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].Settings.PatchAsync(requestBody);


```