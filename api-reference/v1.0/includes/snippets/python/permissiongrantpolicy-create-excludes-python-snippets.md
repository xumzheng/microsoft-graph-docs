---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PermissionGrantConditionSet()
request_body.PermissionType(PermissionType('delegated'))

request_body.resourceApplication = '00000003-0000-0000-c000-000000000000'




result = await client.policies.permissionGrantPolicies_by_id('permissionGrantPolicy-id').excludes.post(request_body = request_body)


```