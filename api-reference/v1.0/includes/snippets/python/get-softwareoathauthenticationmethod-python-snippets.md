---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = SoftwareOathAuthenticationMethodRequestBuilderGetRequestConfiguration(
)


result = await client.me.authentication.softwareOathMethods_by_id('softwareOathAuthenticationMethod-id').get()


```