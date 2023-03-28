---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new UnifiedRoleAssignmentMultipleRequestBuilderGetRequestConfiguration();

$queryParameters = new UnifiedRoleAssignmentMultipleRequestBuilderGetQueryParameters();
$queryParameters.expand = ["roleDefinition","principals","directoryScopes"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.roleManagement().deviceManagement().roleAssignmentsById('unifiedRoleAssignmentMultiple-id').get($requestConfiguration);


```