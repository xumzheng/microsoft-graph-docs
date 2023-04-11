---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = ThreatAssessmentRequestRequestBuilder.ThreatAssessmentRequestRequestBuilderGetQueryParameters(
		expand = ["results"],
)

request_configuration = ThreatAssessmentRequestRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.informationProtection.threatAssessmentRequests_by_id('threatAssessmentRequest-id').get(request_configuration = request_configuration)


```