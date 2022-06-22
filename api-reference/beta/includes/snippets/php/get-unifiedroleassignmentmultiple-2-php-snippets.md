---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new RoleAssignmentsRequestBuilderGetRequestConfiguration();

$queryParameters = new RoleAssignmentsRequestBuilderGetQueryParameters();
$queryParameters->filter%20 = '%20principalIds/any';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->roleManagement()->deviceManagement()->roleAssignments()->get($requestConfiguration);


```