---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new DelegatedAdminAccessAssignment();



$accessContainer = new DelegatedAdminAccessContainer();
$requestRequestBody->setAccessContainer($accessContainer);


$accessContainer->setAccessContainerId('869713c9-0b28-4d08-8949-ae07ae1bf528');
$accessContainer->setAccessContainerType(new DelegatedAdminAccessContainerType('securityGroup'));


$accessDetails = new DelegatedAdminAccessDetails();
$requestRequestBody->setAccessDetails($accessDetails);


$unifiedRolesArray = [];

$unifiedRoles1 = new UnifiedRole();

$unifiedRoles1AdditionalData = [
	"roleDefinitionId" => '29232cdf-9323-42fd-ade2-1d097af3e4de',
];
$unifiedRoles1->setAdditionalData($unifiedRoles1AdditionalData);

$unifiedRolesArray []= $unifiedRoles1;

$unifiedRoles2 = new UnifiedRole();

$unifiedRoles2AdditionalData = [
"roleDefinitionId" => 'f2ef992c-3afb-46b9-b7cf-a126ee74c451',
];
$unifiedRoles2->setAdditionalData($unifiedRoles2AdditionalData);

$unifiedRolesArray []= $unifiedRoles2;

$unifiedRoles3 = new UnifiedRole();

$unifiedRoles3AdditionalData = [
"roleDefinitionId" => '729827e3-9c14-49f7-bb1b-9608f156bbb8',
];
$unifiedRoles3->setAdditionalData($unifiedRoles3AdditionalData);

$unifiedRolesArray []= $unifiedRoles3;

$unifiedRoles4 = new UnifiedRole();

$unifiedRoles4AdditionalData = [
"roleDefinitionId" => '3a2c62db-5318-420d-8d74-23affee5d9d5',
];
$unifiedRoles4->setAdditionalData($unifiedRoles4AdditionalData);

$unifiedRolesArray []= $unifiedRoles4;
$accessDetails->setUnifiedRoles($unifiedRolesArray);

$result =  $graphClient->tenantRelationships()->delegatedAdminRelationshipsById('delegatedAdminRelationship-id')->accessAssignments()->post($requestRequestBody);


```