---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new UserConsentRequestRequestBuilderGetRequestConfiguration();

$queryParameters = new UserConsentRequestRequestBuilderGetQueryParameters();
$queryParameters->filter = '%20';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identityGovernance()->appConsent()->appConsentRequestsById('appConsentRequest-id')->userConsentRequestsById('userConsentRequest-id')->get($requestConfiguration);


```