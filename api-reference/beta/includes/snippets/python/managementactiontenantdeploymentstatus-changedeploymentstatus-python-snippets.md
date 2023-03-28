---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ChangeDeploymentStatusPostRequestBody();
$requestBody->setTenantGroupId('String');

$requestBody->setTenantId('String');

$requestBody->setManagementActionId('String');

$requestBody->setManagementTemplateId('String');

$requestBody->setStatus('String');



$requestResult = $graphServiceClient->tenantRelationships()->managedTenants()->managementActionTenantDeploymentStatuses()->managedTenantsChangeDeploymentStatus()->post($requestBody);


```