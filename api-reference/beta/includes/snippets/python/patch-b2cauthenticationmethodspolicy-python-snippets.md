---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = B2cAuthenticationMethodsPolicy()
request_body.isEmailPasswordAuthenticationEnabled = false

request_body.isUserNameAuthenticationEnabled = true

request_body.isPhoneOneTimePasswordAuthenticationEnabled = true




result = await client.policies.b2cAuthenticationMethodsPolicy.patch(request_body = request_body)


```