---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = ThreatAssessmentRequestRequestBuilderGetRequestConfiguration();

queryParameters = ThreatAssessmentRequestRequestBuilderGetQueryParameters();
queryParameters.expand = ["results"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.informationProtection().threatAssessmentRequestsById('threatAssessmentRequest-id').get(requestConfiguration);


```