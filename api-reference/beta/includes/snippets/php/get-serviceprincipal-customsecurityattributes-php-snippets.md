---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new ServicePrincipalRequestBuilderGetRequestConfiguration();

$queryParameters = new ServicePrincipalRequestBuilderGetQueryParameters();
$queryParameters->select = 'customSecurityAttributes';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->servicePrincipalsById('servicePrincipal-id')->get($requestConfiguration);


```