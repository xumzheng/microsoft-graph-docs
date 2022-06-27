---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new DelegatedAdminRelationship();


$requestRequestBody->setDisplayName('Contoso admin relationship');
$requestRequestBody->setDuration('P730D');

$customer = new DelegatedAdminRelationshipCustomerParticipant();
$requestRequestBody->setCustomer($customer);


$customer->setTenantId('4b827261-d21f-4aa9-b7db-7fa1f56fb163');
$customer->setDisplayName('Contoso subsidiary Inc');


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
"roleDefinitionId" => '3a2c62db-5318-420d-8d74-23affee5d9d5',
];
$unifiedRolesunifiedRoles2->setAdditionalData($unifiedRolesunifiedRoles2AdditionalData);

$unifiedRolesArray []= $unifiedRolesunifiedRoles2;
$accessDetails->setUnifiedRoles($unifiedRolesArray);

$result =  $graphClient->tenantRelationships()->delegatedAdminRelationships()->post($requestRequestBody);


```