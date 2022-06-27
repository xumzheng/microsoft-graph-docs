---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AppConsentRequestRequestBuilderGetRequestConfiguration();

$queryParameters = new AppConsentRequestRequestBuilderGetQueryParameters();
$queryParameters->filter = 'userConsentRequests/any';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identityGovernance()->appConsent()->appConsentRequestsById('appConsentRequest-id')->get($requestConfiguration);


```