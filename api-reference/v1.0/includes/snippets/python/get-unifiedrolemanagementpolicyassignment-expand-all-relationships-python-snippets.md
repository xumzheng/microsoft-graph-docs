---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new UnifiedRoleManagementPolicyAssignmentRequestBuilderGetRequestConfiguration();

$queryParameters = new UnifiedRoleManagementPolicyAssignmentRequestBuilderGetQueryParameters();
$queryParameters->expand = ["policy($expand=rules)"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->policies()->roleManagementPolicyAssignmentsById('unifiedRoleManagementPolicyAssignment-id')->get($requestConfiguration);


```