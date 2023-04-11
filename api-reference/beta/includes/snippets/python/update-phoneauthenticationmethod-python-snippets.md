---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PhoneAuthenticationMethod()
request_body.phoneNumber = '+1 2065555554'

request_body.PhoneType(AuthenticationPhoneType('mobile'))



request_configuration = PhoneAuthenticationMethodRequestBuilderPatchRequestConfiguration(
)


result = await client.me.authentication.phoneMethods_by_id('phoneAuthenticationMethod-id').patch(request_body = request_body)


```