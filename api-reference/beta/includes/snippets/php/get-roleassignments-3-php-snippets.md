---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new RoleAssignmentsRequestBuilderGetRequestConfiguration();

$queryParameters = new RoleAssignmentsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'appScopeId%20eq%20\'/AccessPackageCatalog/4cee616b-fdf9-4890-9d10-955e0ccb12bc\'';
$queryParameters->expand = 'principal';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->roleManagement()->entitlementManagement()->roleAssignments()->get($requestConfiguration);


```