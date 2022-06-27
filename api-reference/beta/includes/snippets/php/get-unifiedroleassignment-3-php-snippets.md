---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new UnifiedRoleAssignmentMultipleRequestBuilderGetRequestConfiguration();

$queryParameters = new UnifiedRoleAssignmentMultipleRequestBuilderGetQueryParameters();
$queryParameters->expand = 'roleDefinition';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->roleManagement()->cloudPC()->roleAssignmentsById('unifiedRoleAssignmentMultiple-id')->get($requestConfiguration);


```