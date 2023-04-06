---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ServicePrincipalRiskDetectionsRequestBuilderGetRequestConfiguration(
request_config = ServicePrincipalRiskDetectionsRequestBuilderGetRequestConfiguration(query_params=params['filter'] = "riskEventType eq 'investigationsThreatIntelligence' or riskLevel eq 'medium'"
)


result = await client.identityProtection.servicePrincipalRiskDetections.get(request_config, headers=request_config)


```