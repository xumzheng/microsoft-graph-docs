---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CrossTenantAccessPolicy()
request_body.setAllowedCloudEndpoints(['microsoftonline.us', ])


request_config = CrossTenantAccessPolicyRequestBuilderPatchRequestConfiguration(
request_config = CrossTenantAccessPolicyRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.policies.crossTenantAccessPolicy.patch(request_body, headers=)


```