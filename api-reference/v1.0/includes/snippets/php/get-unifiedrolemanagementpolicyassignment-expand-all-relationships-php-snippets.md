---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new UnifiedRoleManagementPolicyAssignmentRequestBuilderGetRequestConfiguration();

$queryParameters = new UnifiedRoleManagementPolicyAssignmentRequestBuilderGetQueryParameters();
$queryParameters->expand = 'policy($expand=rules)';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->policies()->roleManagementPolicyAssignmentsById('unifiedRoleManagementPolicyAssignment-id')->get($requestConfiguration);


```