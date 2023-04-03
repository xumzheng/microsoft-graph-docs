---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ApplyPostRequestBody();
requestBody.setTenantId('String');

requestBody.setTenantGroupId('String');

requestBody.setManagementTemplateId('String');



result = await client.tenantRelationships().managedTenants().managementActionsById('managementAction-id').managedTenantsApply().post(requestBody);


```