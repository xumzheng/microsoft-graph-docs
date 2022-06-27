---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ApplyPostRequestBody();


$requestRequestBody->setTenantId('String');
$requestRequestBody->setTenantGroupId('String');
$requestRequestBody->setManagementTemplateId('String');
$result =  $graphClient->tenantRelationships()->managedTenants()->managementActionsById('managementAction-id')->apply()->post($requestRequestBody);


```