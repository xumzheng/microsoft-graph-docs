---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = LanguagesRequestBuilderGetRequestConfiguration(
request_configuration = LanguagesRequestBuilderGetRequestConfiguration(query_params=query_params = LanguagesRequestBuilderGetQueryParameters()
query_params['filter'] = "isEnabled eq true"

)
query_params = LanguagesRequestBuilderGetQueryParameters()
query_params['filter'] = "isEnabled eq true"

)


result = await client.identity.b2cUserFlows_by_id('b2cIdentityUserFlow-id').languages.get(request_configuration)


```