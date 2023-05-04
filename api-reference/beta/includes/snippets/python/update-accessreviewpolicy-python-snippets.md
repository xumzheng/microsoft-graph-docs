---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Access_review_policy()
request_body.is_group_owner_management_enabled = True




result = await client.policies.acces_review_policy.patch(request_body = request_body)


```