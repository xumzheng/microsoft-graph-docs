---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new DevicesRequestBuilderGetRequestConfiguration();

$queryParameters = new DevicesRequestBuilderGetQueryParameters();
$queryParameters->filter = 'startswith(displayName,%20\'a\')';
$queryParameters->count = true;
$queryParameters->top = 1;
$queryParameters->orderby = 'displayName';

$headers = [
"ConsistencyLevel" => "eventual",
];

$requestConfiguration->queryParameters = $queryParameters;
$requestConfiguration->headers = $headers;


$result =  $graphClient->devices()->get($requestConfiguration);


```