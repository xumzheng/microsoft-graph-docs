---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TokenLifetimePolicy()
request_body.Definition(['{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"5:30:00\"}}', ])

request_body.displayName = 'Contoso token lifetime policy'

request_body.isOrganizationDefault = true



request_configuration = TokenLifetimePolicyRequestBuilderPatchRequestConfiguration(
)


result = await client.policies.tokenLifetimePolicies_by_id('tokenLifetimePolicy-id').patch(request_body = request_body)


```