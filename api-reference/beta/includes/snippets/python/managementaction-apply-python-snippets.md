---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ApplyPostRequestBody();
$requestBody->setTenantId('String');

$requestBody->setTenantGroupId('String');

$requestBody->setManagementTemplateId('String');



$requestResult = $graphServiceClient->tenantRelationships()->managedTenants()->managementActionsById('managementAction-id')->managedTenantsApply()->post($requestBody);


```