---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = RiskDetectionsRequestBuilderGetRequestConfiguration();

queryParameters = RiskDetectionsRequestBuilderGetQueryParameters();
queryParameters.filter = "riskEventType eq 'unfamiliarFeatures' or riskLevel eq 'medium'";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.identityProtection().riskDetections().get(requestConfiguration);


```