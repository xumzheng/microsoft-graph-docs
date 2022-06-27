---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new UsersRequestBuilderGetRequestConfiguration();

$queryParameters = new UsersRequestBuilderGetQueryParameters();
$queryParameters->search = '%22displayName:wa%22%20OR%20%22displayName:ad%22';
$queryParameters->orderby = 'displayName';
$queryParameters->count = true;

$headers = [
"ConsistencyLevel" => "eventual",
];

$requestConfiguration->queryParameters = $queryParameters;
$requestConfiguration->headers = $headers;


$result =  $graphClient->users()->get($requestConfiguration);


```