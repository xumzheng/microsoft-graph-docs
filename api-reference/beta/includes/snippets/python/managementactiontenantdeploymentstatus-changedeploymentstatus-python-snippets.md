---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ChangeDeploymentStatusPostRequestBody();
requestBody.setTenantGroupId('String');

requestBody.setTenantId('String');

requestBody.setManagementActionId('String');

requestBody.setManagementTemplateId('String');

requestBody.setStatus('String');



result = await client.tenantRelationships().managedTenants().managementActionTenantDeploymentStatuses().managedTenantsChangeDeploymentStatus().post(requestBody);


```