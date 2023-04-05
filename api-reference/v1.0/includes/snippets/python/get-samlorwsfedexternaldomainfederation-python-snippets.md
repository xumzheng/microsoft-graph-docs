---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = IdentityProviderBaseRequestBuilderGetRequestConfiguration()

query_params = IdentityProviderBaseRequestBuilderGetQueryParameters()
query_params.filter = "domains/any"

request_config.queryParameters = query_params


result = await client.directory_federationConfigurationsby_id('identityProviderBase-id').get(request_config)


```