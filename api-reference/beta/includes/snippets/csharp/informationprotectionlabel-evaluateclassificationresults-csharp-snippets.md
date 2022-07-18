---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EvaluateClassificationResultsRequestBody
{
	ContentInfo = new ContentInfo
	{
		Format = "default",
		Identifier = null,
		State = "rest",
		AdditionalData = new()
		{
			{"@odata.type", "#microsoft.graph.contentInfo"},
			{"format@odata.type", "#microsoft.graph.contentFormat"},
			{"state@odata.type", "#microsoft.graph.contentState"},
		}
	},
	ClassificationResults = new List<ClassificationResult>
	{
		new ClassificationResult
		{
			AdditionalData = new()
			{
				{"sensitiveTypeId", "cb353f78-2b72-4c3c-8827-92ebe4f69fdf"},
				{"count", },
				{"confidenceLevel", },
			}
		},
	}
};
var result = await graphClient.InformationProtection.Policy.Labels.EvaluateClassificationResults.PostAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("User-Agent", "ContosoLOBApp/1.0");
});


```