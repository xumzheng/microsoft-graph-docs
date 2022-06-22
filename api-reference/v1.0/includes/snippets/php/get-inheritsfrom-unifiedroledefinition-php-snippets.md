---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new UnifiedRoleDefinitionRequestBuilderGetRequestConfiguration();

$queryParameters = new UnifiedRoleDefinitionRequestBuilderGetQueryParameters();
$queryParameters->expand = 'inheritsPermissionsFrom';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->roleManagement()->directory()->roleDefinitionsById('unifiedRoleDefinition-id')->get($requestConfiguration);


```