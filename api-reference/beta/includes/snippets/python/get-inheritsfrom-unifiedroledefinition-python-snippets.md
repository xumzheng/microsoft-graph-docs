---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new UnifiedRoleDefinitionRequestBuilderGetRequestConfiguration();

$queryParameters = new UnifiedRoleDefinitionRequestBuilderGetQueryParameters();
$queryParameters->expand = ["inheritsPermissionsFrom"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->roleManagement()->directory()->roleDefinitionsById('unifiedRoleDefinition-id')->get($requestConfiguration);


```