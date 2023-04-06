---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Permission()
request_body.setRoles(['read', ])


request_config = PermissionRequestBuilderPatchRequestConfiguration(
request_config = PermissionRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.sites_by_id('site-id').permissions_by_id('permission-id').patch(request_body, headers=)


```