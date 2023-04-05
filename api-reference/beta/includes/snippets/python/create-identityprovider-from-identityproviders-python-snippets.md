---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityProvider()
request_body.set@odatatype('microsoft.graph.identityProvider')

request_body.setName('Login with Amazon')

request_body.setType('Amazon')

request_body.setClientId('56433757-cadd-4135-8431-2c9e3fd68ae8')

request_body.setClientSecret('000000000000')



result = await client.identityProviders.post(request_body)


```