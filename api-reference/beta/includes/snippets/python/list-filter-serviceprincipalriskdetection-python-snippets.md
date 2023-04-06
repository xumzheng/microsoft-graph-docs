---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = ServicePrincipalRiskDetectionsRequestBuilderGetRequestConfiguration(
request_configuration = ServicePrincipalRiskDetectionsRequestBuilderGetRequestConfiguration(query_params=query_params = ServicePrincipalRiskDetectionsRequestBuilderGetQueryParameters()
query_params['filter'] = "riskEventType eq 'investigationsThreatIntelligence' or riskLevel eq 'medium'"

)
query_params = ServicePrincipalRiskDetectionsRequestBuilderGetQueryParameters()
query_params['filter'] = "riskEventType eq 'investigationsThreatIntelligence' or riskLevel eq 'medium'"

)


result = await client.identityProtection.servicePrincipalRiskDetections.get(request_configuration)


```