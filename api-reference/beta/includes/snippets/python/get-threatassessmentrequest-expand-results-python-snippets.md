---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = ThreatAssessmentRequestRequestBuilderGetRequestConfiguration();

query_params = ThreatAssessmentRequestRequestBuilderGetQueryParameters;
query_params.expand = ["results"];

request_config.queryParameters = query_params;


result = await client.informationProtection().threatAssessmentRequestsById('threatAssessmentRequest-id').get(request_config);


```