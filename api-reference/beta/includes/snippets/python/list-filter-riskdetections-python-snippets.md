---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = RiskDetectionsRequestBuilderGetRequestConfiguration(
request_config = RiskDetectionsRequestBuilderGetRequestConfiguration(query_params=params['filter'] = "riskEventType eq 'unfamiliarFeatures' or riskLevel eq 'medium'"
)


result = await client.identityProtection.riskDetections.get(request_config, headers=request_config)


```