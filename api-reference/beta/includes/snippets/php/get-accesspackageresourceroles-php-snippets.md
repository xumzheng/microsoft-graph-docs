---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AccessPackageResourceRolesRequestBuilderGetRequestConfiguration();

$queryParameters = new AccessPackageResourceRolesRequestBuilderGetQueryParameters();
$queryParameters->filter = '(originSystem%20eq%20\'AadGroup\'%20and%20accessPackageResource/id%20eq%20\'a35bef72-a8aa-4ca3-af30-f6b2ece7208f\')';
$queryParameters->expand = 'accessPackageResource';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageCatalogsById('accessPackageCatalog-id')->accessPackageResourceRoles()->get($requestConfiguration);


```