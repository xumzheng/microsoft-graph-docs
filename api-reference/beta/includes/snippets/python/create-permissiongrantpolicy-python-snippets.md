---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PermissionGrantPolicy()
request_body.id = 'my-custom-consent-policy'

request_body.displayName = 'Custom application consent policy'

request_body.description = 'A custom permission grant policy to customize conditions for granting consent.'




result = await client.policies.permissionGrantPolicies.post(request_body = request_body)


```