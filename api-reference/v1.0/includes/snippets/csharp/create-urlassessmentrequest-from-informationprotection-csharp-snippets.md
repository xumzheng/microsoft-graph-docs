---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ThreatAssessmentRequest
{
	@odata.type = "#microsoft.graph.urlAssessmentRequest",
	ExpectedAssessment = "block",
	Category = "phishing",
	AdditionalData = new()
	{
		{"url", "http://test.com"},
	}
};
var result = await graphClient.InformationProtection.ThreatAssessmentRequests.PostAsync(requestBody);


```