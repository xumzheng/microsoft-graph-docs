---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new RoleAssignmentScheduleRequestsRequestBuilderGetRequestConfiguration();

$queryParameters = new RoleAssignmentScheduleRequestsRequestBuilderGetQueryParameters();
$queryParameters->select = 'principalId,action,roleDefinitionId';
$queryParameters->expand = 'roleDefinition,activatedUsing,principal,targetSchedule';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->roleManagement()->directory()->roleAssignmentScheduleRequests()->get($requestConfiguration);


```