---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new DelegatedAdminRelationship();


$requestRequestBody->setDisplayName('Updated Contoso admin relationship');
$requestRequestBody->setDuration('P31D');

$customer = new DelegatedAdminRelationshipCustomerParticipant();
$requestRequestBody->setCustomer($customer);


$customer->setTenantId('52eaad04-13a2-4a2f-9ce8-93a294fadf36');


$accessDetails = new DelegatedAdminAccessDetails();
$requestRequestBody->setAccessDetails($accessDetails);


$unifiedRolesArray = [];

$unifiedRolesunifiedRoles1 = new UnifiedRole();

$unifiedRolesunifiedRoles1AdditionalData = [
"roleDefinitionId" => '44367163-eba1-44c3-98af-f5787879f96a',
];
$unifiedRolesunifiedRoles1->setAdditionalData($unifiedRolesunifiedRoles1AdditionalData);

$unifiedRolesArray []= $unifiedRolesunifiedRoles1;

$unifiedRolesunifiedRoles2 = new UnifiedRole();

$unifiedRolesunifiedRoles2AdditionalData = [
"roleDefinitionId" => '29232cdf-9323-42fd-ade2-1d097af3e4de',
];
$unifiedRolesunifiedRoles2->setAdditionalData($unifiedRolesunifiedRoles2AdditionalData);

$unifiedRolesArray []= $unifiedRolesunifiedRoles2;

$unifiedRolesunifiedRoles3 = new UnifiedRole();

$unifiedRolesunifiedRoles3AdditionalData = [
"roleDefinitionId" => '69091246-20e8-4a56-aa4d-066075b2a7a8',
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

$requestConfiguration = new DelegatedAdminRelationshipRequestBuilderPatchRequestConfiguration();

$headers = [
"If-Match" => "W/\"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw==\"",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->tenantRelationships()->delegatedAdminRelationshipsById('delegatedAdminRelationship-id')->patch($requestRequestBody, $requestConfiguration);


```