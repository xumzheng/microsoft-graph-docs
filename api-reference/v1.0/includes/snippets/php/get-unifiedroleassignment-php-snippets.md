---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new UnifiedRoleAssignmentRequestBuilderGetRequestConfiguration();

$queryParameters = new UnifiedRoleAssignmentRequestBuilderGetQueryParameters();
$queryParameters->expand = 'roleDefinition';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->roleManagement()->directory()->roleAssignmentsById('unifiedRoleAssignment-id')->get($requestConfiguration);


```