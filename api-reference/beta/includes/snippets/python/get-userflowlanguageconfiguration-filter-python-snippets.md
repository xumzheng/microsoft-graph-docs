---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = LanguagesRequestBuilderGetRequestConfiguration()

query_params = LanguagesRequestBuilderGetQueryParameters()
query_params.filter = "isEnabled eq true"

request_config.queryParameters = query_params


result = await client.identity.b2cUserFlowsById('b2cIdentityUserFlow-id').languages.get(request_config)


```