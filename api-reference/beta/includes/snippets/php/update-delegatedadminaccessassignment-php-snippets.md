---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new DelegatedAdminAccessAssignment();



$accessDetails = new DelegatedAdminAccessDetails();
$requestRequestBody->setAccessDetails($accessDetails);


$unifiedRolesArray = [];

$unifiedRolesunifiedRoles1 = new UnifiedRole();

$unifiedRolesunifiedRoles1AdditionalData = [
	"roleDefinitionId" => '88d8e3e3-8f55-4a1e-953a-9b9898b8876b',
];
$unifiedRolesunifiedRoles1->setAdditionalData($unifiedRolesunifiedRoles1AdditionalData);

$unifiedRolesArray []= $unifiedRolesunifiedRoles1;

$unifiedRolesunifiedRoles2 = new UnifiedRole();

$unifiedRolesunifiedRoles2AdditionalData = [
"roleDefinitionId" => '44367163-eba1-44c3-98af-f5787879f96a',
];
$unifiedRolesunifiedRoles2->setAdditionalData($unifiedRolesunifiedRoles2AdditionalData);

$unifiedRolesArray []= $unifiedRolesunifiedRoles2;

$unifiedRolesunifiedRoles3 = new UnifiedRole();

$unifiedRolesunifiedRoles3AdditionalData = [
"roleDefinitionId" => '729827e3-9c14-49f7-bb1b-9608f156bbb8',
];
$unifiedRolesunifiedRoles3->setAdditionalData($unifiedRolesunifiedRoles3AdditionalData);

$unifiedRolesArray []= $unifiedRolesunifiedRoles3;
$accessDetails->setUnifiedRoles($unifiedRolesArray);

$requestConfiguration = new DelegatedAdminAccessAssignmentRequestBuilderPatchRequestConfiguration();

$headers = [
"If-Match" => "W/\"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw==\"",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->tenantRelationships()->delegatedAdminRelationshipsById('delegatedAdminRelationship-id')->accessAssignmentsById('delegatedAdminAccessAssignment-id')->patch($requestRequestBody, $requestConfiguration);


```