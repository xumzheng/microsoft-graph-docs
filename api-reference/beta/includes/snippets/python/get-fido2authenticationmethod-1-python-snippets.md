---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = Fido2AuthenticationMethodRequestBuilderGetRequestConfiguration(
)


result = await client.me.authentication.fido2Methods_by_id('fido2AuthenticationMethod-id').get()


```