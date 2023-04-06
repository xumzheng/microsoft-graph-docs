---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceCreate()
request_body.set@odataid('https://graph.microsoft.com/beta/identityProviders/{id}')



await client.identity.b2cUserFlows_by_id('b2cIdentityUserFlow-id').identityProviders.ref.post(request_body, headers=)


```