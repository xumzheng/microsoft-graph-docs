---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = EmailAuthenticationMethodRequestBuilderGetRequestConfiguration(
)


result = await client.me.authentication.emailMethods_by_id('emailAuthenticationMethod-id').get()


```