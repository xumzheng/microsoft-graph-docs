---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PhoneAuthenticationMethod()
request_body.setPhoneNumber('+1 2065555554')

request_body.setPhoneType(AuthenticationPhoneType('mobile'))



result = await client.me.authentication.phoneMethodsById('phoneAuthenticationMethod-id').patch(request_body)


```