---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new RoleManagementPolicyAssignmentsRequestBuilderGetRequestConfiguration();

$queryParameters = new RoleManagementPolicyAssignmentsRequestBuilderGetQueryParameters();
$queryParameters->filter = "scopeId eq '/' and scopeType eq 'DirectoryRole' and roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'";
$queryParameters->expand = ["policy($expand=rules)"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->policies()->roleManagementPolicyAssignments()->get($requestConfiguration);


```