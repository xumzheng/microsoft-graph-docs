---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Models.Security.UrlThreatSubmission
{
	OdataType = "#microsoft.graph.urlThreatSubmission",
	Category = Microsoft.Graph.Beta.Models.Security.SubmissionCategory.Phishing,
	WebUrl = "http://phishing.contoso.com",
};
var result = await graphClient.Security.ThreatSubmission.UrlThreats.PostAsync(requestBody);


```