---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = B2cAuthenticationMethodsPolicy();
requestBody.setIsEmailPasswordAuthenticationEnabled(false);

requestBody.setIsUserNameAuthenticationEnabled(true);

requestBody.setIsPhoneOneTimePasswordAuthenticationEnabled(true);



result = await client.policies().b2cAuthenticationMethodsPolicy().patch(requestBody);


```