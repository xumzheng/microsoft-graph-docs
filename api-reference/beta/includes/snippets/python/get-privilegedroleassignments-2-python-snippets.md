---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new PrivilegedRoleAssignmentsRequestBuilderGetRequestConfiguration();

$queryParameters = new PrivilegedRoleAssignmentsRequestBuilderGetQueryParameters();
$queryParameters.filter = "isElevated eq true";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.privilegedRoleAssignments().get($requestConfiguration);


```