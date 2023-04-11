---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthorizationPolicy()
request_body.allowedToUseSSPR = true



request_configuration = AuthorizationPolicyRequestBuilderPatchRequestConfiguration(
)


result = await client.policies.authorizationPolicy_by_id('authorizationPolicy-id').patch(request_body = request_body)


```