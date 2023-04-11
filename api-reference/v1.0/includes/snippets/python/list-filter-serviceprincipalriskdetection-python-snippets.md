---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = ServicePrincipalRiskDetectionsRequestBuilder.ServicePrincipalRiskDetectionsRequestBuilderGetQueryParameters(
				filter = "riskEventType eq 'investigationsThreatIntelligence' or riskLevel eq 'medium'",
)

request_configuration = ServicePrincipalRiskDetectionsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.identityProtection.servicePrincipalRiskDetections.get(request_configuration = request_configuration)


```