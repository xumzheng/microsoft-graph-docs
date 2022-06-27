---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TenantTag();


$requestRequestBody->setDisplayName('Support');
$requestRequestBody->setDescription('Tenants that have purchased extended support');
$result =  $graphClient->tenantRelationships()->managedTenants()->tenantTags()->post($requestRequestBody);


```