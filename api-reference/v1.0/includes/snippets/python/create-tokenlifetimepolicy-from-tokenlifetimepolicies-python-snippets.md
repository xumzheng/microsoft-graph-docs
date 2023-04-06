---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TokenLifetimePolicy()
request_body.setDefinition(['{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}', ])

request_body.setDisplayName('Contoso token lifetime policy')

request_body.setIsOrganizationDefault(true)



result = await client.policies.tokenLifetimePolicies.post(request_body, headers=)


```