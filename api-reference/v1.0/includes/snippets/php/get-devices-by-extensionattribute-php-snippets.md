---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new DevicesRequestBuilderGetRequestConfiguration();

$queryParameters = new DevicesRequestBuilderGetQueryParameters();
$queryParameters->filter = 'extensionAttributes/extensionAttribute1%20eq%20\'BYOD-Device\'';
$queryParameters->count = true;

$headers = [
"ConsistencyLevel" => "eventual",
];

$requestConfiguration->queryParameters = $queryParameters;
$requestConfiguration->headers = $headers;


$result =  $graphClient->devices()->get($requestConfiguration);


```