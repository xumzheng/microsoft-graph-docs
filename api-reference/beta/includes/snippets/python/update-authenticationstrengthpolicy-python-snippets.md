---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthenticationStrengthPolicy()
request_body.@odatatype = '#microsoft.graph.authenticationStrengthPolicy'

request_body.displayName = 'FIDO2 only'

request_body.description = 'An auth strength allowing only FIDO2 security keys.'



request_configuration = AuthenticationStrengthPolicyRequestBuilderPatchRequestConfiguration(
)


result = await client.policies.authenticationStrengthPolicies_by_id('authenticationStrengthPolicy-id').patch(request_body = request_body)


```