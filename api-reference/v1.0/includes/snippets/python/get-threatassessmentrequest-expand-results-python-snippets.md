---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ThreatAssessmentRequestRequestBuilderGetRequestConfiguration(
query_params = ThreatAssessmentRequestRequestBuilderGetQueryParameters()
query_params.expand = ["results"]

)


result = await client.informationProtection.threatAssessmentRequests_by_id('threatAssessmentRequest-id').get(request_config)


```