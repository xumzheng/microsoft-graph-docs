---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = TenantTag();
requestBody.setDisplayName('Support');

requestBody.setDescription('Tenants that have purchased extended support');



result = await client.tenantRelationships().managedTenants().tenantTags().post(requestBody);


```