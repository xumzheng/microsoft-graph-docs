---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new TransitiveRoleAssignmentsRequestBuilderGetRequestConfiguration();

$queryParameters = new TransitiveRoleAssignmentsRequestBuilderGetQueryParameters();
$queryParameters->count = true;
$queryParameters->filter = 'principalId%20eq%20\'2c7936bc-3517-40f3-8eda-4806637b6516\'';

$headers = [
"ConsistencyLevel" => "eventual",
];

$requestConfiguration->queryParameters = $queryParameters;
$requestConfiguration->headers = $headers;


$result =  $graphClient->roleManagement()->directory()->transitiveRoleAssignments()->get($requestConfiguration);


```