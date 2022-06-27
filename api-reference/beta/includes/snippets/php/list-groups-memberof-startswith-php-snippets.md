---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new GroupRequestBuilderGetRequestConfiguration();

$queryParameters = new GroupRequestBuilderGetQueryParameters();
$queryParameters->count = true;
$queryParameters->orderby = 'displayName';
$queryParameters->filter = 'startswith(displayName,%20\'A\')';

$headers = [
"ConsistencyLevel" => "eventual",
];

$requestConfiguration->queryParameters = $queryParameters;
$requestConfiguration->headers = $headers;


$result =  $graphClient->groupsById('group-id')->memberOf()->group()->get($requestConfiguration);


```