---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PermissionGrantConditionSet()
request_body.setPermissionType(PermissionType('delegated'))

request_body.setResourceApplication('00000003-0000-0000-c000-000000000000')



result = await client.policies.permissionGrantPoliciesby_id('permissionGrantPolicy-id').excludes.post(request_body)


```