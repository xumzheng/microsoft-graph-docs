---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TenantIdRequestBody();


$requestRequestBody->setTenantId('String');
$result =  $graphClient->tenantRelationships()->managedTenants()->tenantGroups()->tenantSearch()->post($requestRequestBody);


```