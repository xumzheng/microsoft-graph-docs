---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new GroupsRequestBuilderGetRequestConfiguration();

$queryParameters = new GroupsRequestBuilderGetQueryParameters();
$queryParameters->search = '%22displayName:Video%22%20OR%20%22description:prod%22';
$queryParameters->orderby = 'displayName';
$queryParameters->count = true;

$headers = [
"ConsistencyLevel" => "eventual",
];

$requestConfiguration->queryParameters = $queryParameters;
$requestConfiguration->headers = $headers;


$result =  $graphClient->groups()->get($requestConfiguration);


```