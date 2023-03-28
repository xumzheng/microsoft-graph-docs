---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new AppConsentRequestRequestBuilderGetRequestConfiguration();

$queryParameters = new AppConsentRequestRequestBuilderGetQueryParameters();
$queryParameters->filter = "userConsentRequests/any";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->identityGovernance()->appConsent()->appConsentRequestsById('appConsentRequest-id')->get($requestConfiguration);


```