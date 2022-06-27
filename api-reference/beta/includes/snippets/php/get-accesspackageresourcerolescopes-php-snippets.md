---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AccessPackageRequestBuilderGetRequestConfiguration();

$queryParameters = new AccessPackageRequestBuilderGetQueryParameters();
$queryParameters->expand = 'accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackagesById('accessPackage-id')->get($requestConfiguration);


```