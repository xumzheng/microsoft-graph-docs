---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new RiskyUsersRequestBuilderGetRequestConfiguration();

$queryParameters = new RiskyUsersRequestBuilderGetQueryParameters();
$queryParameters->filter = 'riskLevel%20eq%20microsoft.graph.riskLevel\'medium\'';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identityProtection()->riskyUsers()->get($requestConfiguration);


```