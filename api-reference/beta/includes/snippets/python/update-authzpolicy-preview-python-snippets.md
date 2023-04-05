---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthorizationPolicy()
request_body.setEnabledPreviewFeatures(['assignGroupsToRoles', ])



result = await client.policies.authorizationPolicyby_id('authorizationPolicy-id').patch(request_body)


```