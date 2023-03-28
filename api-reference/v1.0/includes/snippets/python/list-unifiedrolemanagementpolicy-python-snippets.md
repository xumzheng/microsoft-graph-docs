---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new RoleManagementPoliciesRequestBuilderGetRequestConfiguration();

$queryParameters = new RoleManagementPoliciesRequestBuilderGetQueryParameters();
$queryParameters.filter = "scopeId eq '/' and scopeType eq 'DirectoryRole'";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.policies().roleManagementPolicies().get($requestConfiguration);


```