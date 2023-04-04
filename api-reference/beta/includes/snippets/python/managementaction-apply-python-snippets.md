---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ApplyPostRequestBody()
request_body.setTenantId('String')

request_body.setTenantGroupId('String')

request_body.setManagementTemplateId('String')



result = await client.tenantRelationships.managedTenants.managementActionsById('managementAction-id').managedTenantsapply.post(request_body)


```