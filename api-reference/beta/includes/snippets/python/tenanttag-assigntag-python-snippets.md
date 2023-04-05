---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AssignTagPostRequestBody()
request_body.setTenantIds(['String', ])



result = await client.tenantRelationships.managedTenants.tenantTagsby_id('tenantTag-id').managedTenantsassignTag.post(request_body)


```