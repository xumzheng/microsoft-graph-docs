---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new AppConsentRequestsRequestBuilderGetRequestConfiguration();

$queryParameters = new AppConsentRequestsRequestBuilderGetQueryParameters();
$queryParameters.filter = "userConsentRequests/any ";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.identityGovernance().appConsent().appConsentRequests().get($requestConfiguration);


```