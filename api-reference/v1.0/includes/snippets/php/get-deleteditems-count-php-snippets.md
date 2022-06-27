---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new GroupRequestBuilderGetRequestConfiguration();

$queryParameters = new GroupRequestBuilderGetQueryParameters();
$queryParameters->count = true;
$queryParameters->orderBy = 'deletedDateTime%20asc';
$queryParameters->select = 'id,DisplayName,deletedDateTime';

$headers = [
"ConsistencyLevel" => "eventual",
];

$requestConfiguration->queryParameters = $queryParameters;
$requestConfiguration->headers = $headers;


$result =  $graphClient->directory()->deletedItems()->group()->get($requestConfiguration);


```