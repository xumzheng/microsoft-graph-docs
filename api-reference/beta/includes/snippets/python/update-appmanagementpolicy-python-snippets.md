---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AppManagementPolicy()
request_body.isEnabled = false




result = await client.policies.appManagementPolicies_by_id('appManagementPolicy-id').patch(request_body = request_body)


```