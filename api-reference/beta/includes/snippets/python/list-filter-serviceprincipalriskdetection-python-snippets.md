---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ServicePrincipalRiskDetectionsRequestBuilderGetRequestConfiguration()

query_params = ServicePrincipalRiskDetectionsRequestBuilderGetQueryParameters()
query_params.filter = "riskEventType eq 'investigationsThreatIntelligence' or riskLevel eq 'medium'"

request_config.queryParameters = query_params


result = await client.identityProtection_servicePrincipalRiskDetections.get(request_config)


```