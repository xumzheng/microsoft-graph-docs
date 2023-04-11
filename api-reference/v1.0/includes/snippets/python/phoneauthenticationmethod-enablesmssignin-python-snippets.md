---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = EnableSmsSignInRequestBuilderPostRequestConfiguration(
)


await client.me.authentication.phoneMethods_by_id('phoneAuthenticationMethod-id').enableSmsSignIn.post()


```