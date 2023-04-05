---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChangeDeploymentStatusPostRequestBody()
request_body.setTenantGroupId('String')

request_body.setTenantId('String')

request_body.setManagementActionId('String')

request_body.setManagementTemplateId('String')

request_body.setStatus('String')



result = await client.tenantRelationships_managedTenants_managementActionTenantDeploymentStatuses_managedTenantschangeDeploymentStatus.post(request_body)


```