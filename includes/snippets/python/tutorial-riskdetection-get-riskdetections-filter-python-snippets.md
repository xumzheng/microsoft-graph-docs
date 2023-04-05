---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = RiskDetectionsRequestBuilderGetRequestConfiguration(
query_params = RiskDetectionsRequestBuilderGetQueryParameters()
query_params.filter = "userDisplayName eq 'MyTestUser1'"

)


result = await client.identityProtection.riskDetections.get(request_config)


```