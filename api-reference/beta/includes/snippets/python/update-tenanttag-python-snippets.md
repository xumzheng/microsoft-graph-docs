---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new TenantTag();
$requestBody->setDisplayName('Onboarding');

$requestBody->setDescription('Tenants that we are currently onboarding');



$requestResult = $graphServiceClient->tenantRelationships()->managedTenants()->tenantTagsById('tenantTag-id')->patch($requestBody);


```