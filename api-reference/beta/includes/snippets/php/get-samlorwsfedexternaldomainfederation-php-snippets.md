---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new IdentityProviderBaseRequestBuilderGetRequestConfiguration();

$queryParameters = new IdentityProviderBaseRequestBuilderGetQueryParameters();
$queryParameters->filter = 'domains/any';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->directory()->federationConfigurationsById('identityProviderBase-id')->get($requestConfiguration);


```