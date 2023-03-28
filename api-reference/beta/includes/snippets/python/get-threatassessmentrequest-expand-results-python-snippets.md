---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new ThreatAssessmentRequestRequestBuilderGetRequestConfiguration();

$queryParameters = new ThreatAssessmentRequestRequestBuilderGetQueryParameters();
$queryParameters.expand = ["results"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.informationProtection().threatAssessmentRequestsById('threatAssessmentRequest-id').get($requestConfiguration);


```