---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.IdentityProtection.ServicePrincipalRiskDetections.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Filter = "riskEventType eq 'investigationsThreatIntelligence' or riskLevel eq 'medium'";
});


```