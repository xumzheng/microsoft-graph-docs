---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AccessPackageResourceRolesRequestBuilderGetRequestConfiguration();

$queryParameters = new AccessPackageResourceRolesRequestBuilderGetQueryParameters();
$queryParameters->filter = '(originSystem%20eq%20\'SharePointOnline\'%20and%20accessPackageResource/id%20eq%20\'53c71803-a0a8-4777-aecc-075de8ee3991\')';
$queryParameters->select = 'displayName,originId';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageCatalogsById('accessPackageCatalog-id')->accessPackageResourceRoles()->get($requestConfiguration);


```