---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AccessPackageResourceEnvironmentsRequestBuilderGetRequestConfiguration();

$queryParameters = new AccessPackageResourceEnvironmentsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'originSystem%20eq%20\'SharePointOnline\'';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageResourceEnvironments()->get($requestConfiguration);


```