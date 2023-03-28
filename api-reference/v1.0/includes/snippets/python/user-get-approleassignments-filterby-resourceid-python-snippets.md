---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new AppRoleAssignmentsRequestBuilderGetRequestConfiguration();

$queryParameters = new AppRoleAssignmentsRequestBuilderGetQueryParameters();
$queryParameters.filter = "resourceId eq 8e881353-1735-45af-af21-ee1344582a4d";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.usersById('user-id').appRoleAssignments().get($requestConfiguration);


```