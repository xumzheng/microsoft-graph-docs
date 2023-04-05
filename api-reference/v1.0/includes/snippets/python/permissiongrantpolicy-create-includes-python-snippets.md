---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PermissionGrantConditionSet()
request_body.setPermissionType(PermissionType('delegated'))

request_body.setClientApplicationsFromVerifiedPublisherOnly(true)



result = await client.policies.permissionGrantPolicies._by_id('permissionGrantPolicy-id').includes.post(request_body)


```