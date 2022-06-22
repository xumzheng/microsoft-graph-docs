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

$unifiedRoles1 = new UnifiedRole();

$unifiedRoles1AdditionalData = [
	"roleDefinitionId" => '44367163-eba1-44c3-98af-f5787879f96a',
];
$unifiedRoles1->setAdditionalData($unifiedRoles1AdditionalData);

$unifiedRolesArray []= $unifiedRoles1;

$unifiedRoles2 = new UnifiedRole();

$unifiedRoles2AdditionalData = [
"roleDefinitionId" => '29232cdf-9323-42fd-ade2-1d097af3e4de',
];
$unifiedRoles2->setAdditionalData($unifiedRoles2AdditionalData);

$unifiedRolesArray []= $unifiedRoles2;

$unifiedRoles3 = new UnifiedRole();

$unifiedRoles3AdditionalData = [
"roleDefinitionId" => '69091246-20e8-4a56-aa4d-066075b2a7a8',
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

$requestConfiguration = new DelegatedAdminRelationshipRequestBuilderPatchRequestConfiguration();

$headers = [
"If-Match" => "W/\"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw==\"",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->tenantRelationships()->delegatedAdminRelationshipsById('delegatedAdminRelationship-id')->patch($requestRequestBody, $requestConfiguration);


```