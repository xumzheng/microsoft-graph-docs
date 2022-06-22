---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AppConsentRequestsRequestBuilderGetRequestConfiguration();

$queryParameters = new AppConsentRequestsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'userConsentRequests/any%20';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identityGovernance()->appConsent()->appConsentRequests()->get($requestConfiguration);


```