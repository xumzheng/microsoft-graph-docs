---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ThreatAssessmentRequest
{
	@odata.type = "#microsoft.graph.emailFileAssessmentRequest",
	ExpectedAssessment = "block",
	Category = "malware",
	AdditionalData = new()
	{
		{"recipientEmail", "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com"},
		{"contentData", "UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC....."},
	}
};
var result = await graphClient.InformationProtection.ThreatAssessmentRequests.PostAsync(requestBody);


```