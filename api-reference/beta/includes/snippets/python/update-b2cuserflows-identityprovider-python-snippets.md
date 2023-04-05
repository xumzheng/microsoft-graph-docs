---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceCreate()
request_body.set@odataid('https://graph.microsoft.com/beta/identityProviders/{id}')



await client.identity_b2cUserFlowsby_id('b2cIdentityUserFlow-id')_identityProviders_ref.post(request_body)


```