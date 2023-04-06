---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PermissionGrantPolicy()
request_body.setDisplayName('Custom permission grant policy')


request_config = PermissionGrantPolicyRequestBuilderPatchRequestConfiguration(
request_config = PermissionGrantPolicyRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.policies.permissionGrantPolicies_by_id('permissionGrantPolicy-id').patch(request_body, headers=)


```