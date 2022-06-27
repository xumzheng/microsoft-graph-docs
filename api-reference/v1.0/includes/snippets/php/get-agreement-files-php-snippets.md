---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AgreementRequestBuilderGetRequestConfiguration();

$queryParameters = new AgreementRequestBuilderGetQueryParameters();
$queryParameters->expand = 'files';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identityGovernance()->termsOfUse()->agreementsById('agreement-id')->get($requestConfiguration);


```