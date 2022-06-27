---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new GroupRequestBuilderGetRequestConfiguration();

$queryParameters = new GroupRequestBuilderGetQueryParameters();
$queryParameters->count = true;

$headers = [
"ConsistencyLevel" => "eventual",
];

$requestConfiguration->queryParameters = $queryParameters;
$requestConfiguration->headers = $headers;


$result =  $graphClient->groupsById('group-id')->transitiveMembers()->group()->get($requestConfiguration);


```