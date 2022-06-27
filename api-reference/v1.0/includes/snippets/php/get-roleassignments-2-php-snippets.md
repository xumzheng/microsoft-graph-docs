---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new RoleAssignmentsRequestBuilderGetRequestConfiguration();

$queryParameters = new RoleAssignmentsRequestBuilderGetQueryParameters();
$queryParameters->filter%20 = '%20principalId%20eq%20\'f1847572-48aa-47aa-96a3-2ec61904f41f\'';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->roleManagement()->directory()->roleAssignments()->get($requestConfiguration);


```