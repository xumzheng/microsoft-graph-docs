---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = PasswordAuthenticationMethodRequestBuilderGetRequestConfiguration(
)


result = await client.me.authentication.passwordMethods_by_id('passwordAuthenticationMethod-id').get()


```