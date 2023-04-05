---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = LanguagesRequestBuilderGetRequestConfiguration()

query_params = LanguagesRequestBuilderGetQueryParameters()
query_params.filter = "isEnabled eq true"

request_config.queryParameters = query_params


result = await client.identity_b2cUserFlowsby_id('b2cIdentityUserFlow-id')_languages.get(request_config)


```