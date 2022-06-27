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

$unifiedRolesunifiedRoles1 = new UnifiedRole();

$unifiedRolesunifiedRoles1AdditionalData = [
"roleDefinitionId" => '29232cdf-9323-42fd-ade2-1d097af3e4de',
];
$unifiedRolesunifiedRoles1->setAdditionalData($unifiedRolesunifiedRoles1AdditionalData);

$unifiedRolesArray []= $unifiedRolesunifiedRoles1;

$unifiedRolesunifiedRoles2 = new UnifiedRole();

$unifiedRolesunifiedRoles2AdditionalData = [
"roleDefinitionId" => 'f2ef992c-3afb-46b9-b7cf-a126ee74c451',
];
$unifiedRolesunifiedRoles2->setAdditionalData($unifiedRolesunifiedRoles2AdditionalData);

$unifiedRolesArray []= $unifiedRolesunifiedRoles2;

$unifiedRolesunifiedRoles3 = new UnifiedRole();

$unifiedRolesunifiedRoles3AdditionalData = [
"roleDefinitionId" => '729827e3-9c14-49f7-bb1b-9608f156bbb8',
];
$unifiedRolesunifiedRoles3->setAdditionalData($unifiedRolesunifiedRoles3AdditionalData);

$unifiedRolesArray []= $unifiedRolesunifiedRoles3;

$unifiedRolesunifiedRoles4 = new UnifiedRole();

$unifiedRolesunifiedRoles4AdditionalData = [
"roleDefinitionId" => '3a2c62db-5318-420d-8d74-23affee5d9d5',
];
$unifiedRolesunifiedRoles4->setAdditionalData($unifiedRolesunifiedRoles4AdditionalData);

$unifiedRolesArray []= $unifiedRolesunifiedRoles4;
$accessDetails->setUnifiedRoles($unifiedRolesArray);

$result =  $graphClient->tenantRelationships()->delegatedAdminRelationshipsById('delegatedAdminRelationship-id')->accessAssignments()->post($requestRequestBody);


```