---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PhoneAuthenticationMethod()
request_body.phoneNumber = '+1 2065555555'

request_body.PhoneType(AuthenticationPhoneType('mobile'))



request_configuration = PhoneMethodsRequestBuilderPostRequestConfiguration(
)


result = await client.me.authentication.phoneMethods.post(request_body = request_body)


```