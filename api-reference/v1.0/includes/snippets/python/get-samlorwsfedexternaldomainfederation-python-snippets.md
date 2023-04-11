---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = IdentityProviderBaseRequestBuilder.IdentityProviderBaseRequestBuilderGetQueryParameters(
				filter = "domains/any",
)

request_configuration = IdentityProviderBaseRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.directory.federationConfigurations_by_id('identityProviderBase-id').get(request_configuration = request_configuration)


```