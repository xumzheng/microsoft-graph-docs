---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new ServicePrincipalsRequestBuilderGetRequestConfiguration();

$queryParameters = new ServicePrincipalsRequestBuilderGetQueryParameters();
$queryParameters->search = '%22displayName:Team%22';
$queryParameters->count = true;

$headers = [
"ConsistencyLevel" => "eventual",
];

$requestConfiguration->queryParameters = $queryParameters;
$requestConfiguration->headers = $headers;


$result =  $graphClient->servicePrincipals()->get($requestConfiguration);


```