---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = B2cAuthenticationMethodsPolicy()
request_body.setIsEmailPasswordAuthenticationEnabled(false)

request_body.setIsUserNameAuthenticationEnabled(true)

request_body.setIsPhoneOneTimePasswordAuthenticationEnabled(true)



result = await client.policies_b2cAuthenticationMethodsPolicy.patch(request_body)


```