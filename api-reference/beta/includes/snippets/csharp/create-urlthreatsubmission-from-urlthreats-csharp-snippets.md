---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UrlThreatSubmission
{
	OdataType = "#microsoft.graph.urlThreatSubmission",
	Category = SubmissionCategory.Phishing,
	WebUrl = "http://phishing.contoso.com",
};
var result = await graphClient.Security.ThreatSubmission.UrlThreats.PostAsync(requestBody);


```