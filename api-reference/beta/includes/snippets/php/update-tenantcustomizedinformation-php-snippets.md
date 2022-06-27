---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TenantCustomizedInformation();


$requestRequestBody->setTenantId('String');
$contactsArray = [];

$contactscontacts1 = new TenantContactInformation();

$contactscontacts1->setName('String');
$contactscontacts1->setTitle('String');
$contactscontacts1->setEmail('String');
$contactscontacts1->setPhone('String');
$contactscontacts1->setNotes('String');
$contactscontacts1AdditionalData = [
	"@odata.type" => 'microsoft.graph.managedTenants.tenantContactInformation',
];
$contactscontacts1->setAdditionalData($contactscontacts1AdditionalData);

$contactsArray []= $contactscontacts1;
$requestRequestBody->setContacts($contactsArray);
$requestRequestBody->setWebsite('String');
$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.managedTenants.tenantCustomizedInformation',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->tenantRelationships()->managedTenants()->tenantsCustomizedInformationById('tenantCustomizedInformation-id')->patch($requestRequestBody);


```