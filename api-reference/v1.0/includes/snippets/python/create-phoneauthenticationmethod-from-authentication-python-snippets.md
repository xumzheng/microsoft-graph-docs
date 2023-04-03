---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PhoneAuthenticationMethod();
requestBody.setPhoneNumber('+1 2065555555');

requestBody.setPhoneType(AuthenticationPhoneType('mobile'));



result = awaitclient.me().authentication().phoneMethods().post(requestBody);


```