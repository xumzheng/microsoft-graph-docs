---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new TenantCustomizedInformation();
$requestBody->set@odatatype('#microsoft.graph.managedTenants.tenantCustomizedInformation');

$requestBody->setTenantId('String');

$contactsTenantContactInformation1 = new TenantContactInformation();
$contactsTenantContactInformation1->set@odatatype('microsoft.graph.managedTenants.tenantContactInformation');

$contactsTenantContactInformation1->setName('String');

$contactsTenantContactInformation1->setTitle('String');

$contactsTenantContactInformation1->setEmail('String');

$contactsTenantContactInformation1->setPhone('String');

$contactsTenantContactInformation1->setNotes('String');


$contactsArray []= $contactsTenantContactInformation1;
$requestBody->setContacts($contactsArray);


$requestBody->setWebsite('String');



$requestResult = $graphServiceClient->tenantRelationships()->managedTenants()->tenantsCustomizedInformationById('tenantCustomizedInformation-id')->patch($requestBody);


```