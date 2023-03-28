---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new PrivilegedRoleAssignmentsRequestBuilderGetRequestConfiguration();

$queryParameters = new PrivilegedRoleAssignmentsRequestBuilderGetQueryParameters();
$queryParameters.filter = "isElevated eq true and expirationDateTime ne null or isElevated eq false";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.privilegedRoleAssignments().get($requestConfiguration);


```