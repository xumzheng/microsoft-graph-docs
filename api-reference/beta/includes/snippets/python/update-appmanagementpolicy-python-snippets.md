---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AppManagementPolicy()
request_body.setIsEnabled(false)



result = await client.policies_appManagementPoliciesby_id('appManagementPolicy-id').patch(request_body)


```