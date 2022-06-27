---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AccessPackageResourcesRequestBuilderGetRequestConfiguration();

$queryParameters = new AccessPackageResourcesRequestBuilderGetQueryParameters();
$queryParameters->filter = 'resourceType%20eq%20\'Application\'';
$queryParameters->expand = 'accessPackageResourceScopes';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageCatalogsById('accessPackageCatalog-id')->accessPackageResources()->get($requestConfiguration);


```