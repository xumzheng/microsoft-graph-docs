---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedRoleAssignment();


$requestRequestBody->setPrincipalId('679a9213-c497-48a4-830a-8d3d25d94ddc');
$requestRequestBody->setRoleDefinitionId('ae79f266-94d4-4dab-b730-feca7e132178');
$requestRequestBody->setAppScopeId('/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997');
$result =  $graphClient->roleManagement()->entitlementManagement()->roleAssignments()->post($requestRequestBody);


```