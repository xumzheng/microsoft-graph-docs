---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TenantCustomizedInformation();


$requestRequestBody->setTenantId('String');
$contactsArray = [];

$contacts1 = new TenantContactInformation();

$contacts1->setName('String');
$contacts1->setTitle('String');
$contacts1->setEmail('String');
$contacts1->setPhone('String');
$contacts1->setNotes('String');
$contacts1AdditionalData = [
		"@odata.type" => 'microsoft.graph.managedTenants.tenantContactInformation',
	];
$contacts1->setAdditionalData($contacts1AdditionalData);

$contactsArray []= $contacts1;
$requestRequestBody->setContacts($contactsArray);
$requestRequestBody->setWebsite('String');
$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.managedTenants.tenantCustomizedInformation',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->tenantRelationships()->managedTenants()->tenantsCustomizedInformationById('tenantCustomizedInformation-id')->patch($requestRequestBody);


```