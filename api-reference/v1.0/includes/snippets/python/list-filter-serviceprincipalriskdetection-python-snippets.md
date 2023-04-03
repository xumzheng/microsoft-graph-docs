---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = ServicePrincipalRiskDetectionsRequestBuilderGetRequestConfiguration();

queryParameters = ServicePrincipalRiskDetectionsRequestBuilderGetQueryParameters();
queryParameters.filter = "riskEventType eq 'investigationsThreatIntelligence' or riskLevel eq 'medium'";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.identityProtection().servicePrincipalRiskDetections().get(requestConfiguration);


```