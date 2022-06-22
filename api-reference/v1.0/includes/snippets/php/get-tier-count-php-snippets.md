---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new UserRequestBuilderGetRequestConfiguration();

$queryParameters = new UserRequestBuilderGetQueryParameters();
$queryParameters->count = true;
$queryParameters->orderBy = 'displayName';
$queryParameters->search = '%22displayName:tier%22';
$queryParameters->select = 'displayName,id';

$headers = [
"ConsistencyLevel" => "eventual",
];

$requestConfiguration->queryParameters = $queryParameters;
$requestConfiguration->headers = $headers;


$result =  $graphClient->groupsById('group-id')->transitiveMembers()->user()->get($requestConfiguration);


```