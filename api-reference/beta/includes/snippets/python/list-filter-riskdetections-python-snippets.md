---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = RiskDetectionsRequestBuilderGetRequestConfiguration();

query_params = RiskDetectionsRequestBuilderGetQueryParameters();
query_params.filter = "riskEventType eq 'unfamiliarFeatures' or riskLevel eq 'medium'";

request_config.queryParameters = query_params;


result = await client.identityProtection.riskDetections.get(request_config);


```