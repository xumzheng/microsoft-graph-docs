---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PhoneAuthenticationMethod();
requestBody.setPhoneNumber('+1 2065555554');

requestBody.setPhoneType(AuthenticationPhoneType('mobile'));



result = awaitclient.me().authentication().phoneMethodsById('phoneAuthenticationMethod-id').patch(requestBody);


```