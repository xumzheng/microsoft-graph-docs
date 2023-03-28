---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new RoleAssignmentsRequestBuilderGetRequestConfiguration();

$queryParameters = new RoleAssignmentsRequestBuilderGetQueryParameters();
$queryParameters.filter = " principalIds/any";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.roleManagement().deviceManagement().roleAssignments().get($requestConfiguration);


```