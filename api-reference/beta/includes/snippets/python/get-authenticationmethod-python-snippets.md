---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = AuthenticationMethodRequestBuilderGetRequestConfiguration(
)


result = await client.me.authentication.methods_by_id('authenticationMethod-id').get()


```