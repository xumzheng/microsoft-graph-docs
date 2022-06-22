---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ChangeDeploymentStatusPostRequestBody();


$requestRequestBody->setTenantGroupId('String');
$requestRequestBody->setTenantId('String');
$requestRequestBody->setManagementActionId('String');
$requestRequestBody->setManagementTemplateId('String');
$requestRequestBody->setStatus('String');
$result =  $graphClient->tenantRelationships()->managedTenants()->managementActionTenantDeploymentStatuses()->changeDeploymentStatus()->post($requestRequestBody);


```