---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PhoneAuthenticationMethod()
request_body.setPhoneNumber('+1 2065555555')

request_body.setPhoneType(AuthenticationPhoneType('mobile'))


request_config = PhoneMethodsRequestBuilderPostRequestConfiguration(
request_config = PhoneMethodsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.me.authentication.phoneMethods.post(request_body, headers=)


```