---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthenticationStrengthPolicy()
request_body.set@odatatype('#microsoft.graph.authenticationStrengthPolicy')

request_body.setDisplayName('FIDO2 only')

request_body.setDescription('An auth strength allowing only FIDO2 security keys.')



result = await client.policies.authenticationStrengthPoliciesById('authenticationStrengthPolicy-id').patch(request_body)


```