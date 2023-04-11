---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentitySecurityDefaultsEnforcementPolicy()
request_body.isEnabled = false



request_configuration = IdentitySecurityDefaultsEnforcementPolicyRequestBuilderPatchRequestConfiguration(
)


result = await client.policies.identitySecurityDefaultsEnforcementPolicy.patch(request_body = request_body)


```