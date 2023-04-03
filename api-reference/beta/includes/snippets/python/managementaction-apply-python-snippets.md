---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ApplyPostRequestBody();
requestBody.setTenantId('String');

requestBody.setTenantGroupId('String');

requestBody.setManagementTemplateId('String');



result = awaitclient.tenantRelationships().managedTenants().managementActionsById('managementAction-id').managedTenantsApply().post(requestBody);


```