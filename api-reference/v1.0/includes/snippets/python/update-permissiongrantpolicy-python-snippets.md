---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PermissionGrantPolicy()
request_body.displayName = 'Custom permission grant policy'



request_configuration = PermissionGrantPolicyRequestBuilderPatchRequestConfiguration(
)


result = await client.policies.permissionGrantPolicies_by_id('permissionGrantPolicy-id').patch(request_body = request_body)


```