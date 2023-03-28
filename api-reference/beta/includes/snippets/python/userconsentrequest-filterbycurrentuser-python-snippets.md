---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new UserConsentRequestRequestBuilderGetRequestConfiguration();

$queryParameters = new UserConsentRequestRequestBuilderGetQueryParameters();
$queryParameters->filter = " ";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->identityGovernance()->appConsent()->appConsentRequestsById('appConsentRequest-id')->userConsentRequestsById('userConsentRequest-id')->get($requestConfiguration);


```