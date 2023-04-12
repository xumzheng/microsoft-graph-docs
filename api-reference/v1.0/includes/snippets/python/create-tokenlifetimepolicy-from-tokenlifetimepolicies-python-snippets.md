---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TokenLifetimePolicy()
request_body.Definition(['{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}', ])

request_body.displayName = 'Contoso token lifetime policy'

request_body.isOrganizationDefault = true




result = await client.policies.tokenLifetimePolicies.post(request_body = request_body)


```