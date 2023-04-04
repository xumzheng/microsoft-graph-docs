---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = UnassignTagPostRequestBody();
request_body.setTenantIds(['String', ]);



result = await client.tenantRelationships().managedTenants().tenantTagsById('tenantTag-id').managedTenantsUnassignTag().post(request_body);


```