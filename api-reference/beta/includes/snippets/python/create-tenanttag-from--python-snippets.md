---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TenantTag()
request_body.setDisplayName('Support')

request_body.setDescription('Tenants that have purchased extended support')



result = await client.tenantRelationships_managedTenants_tenantTags.post(request_body)


```