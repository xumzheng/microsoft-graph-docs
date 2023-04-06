---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = DefinitionsRequestBuilderGetRequestConfiguration(
request_configuration = DefinitionsRequestBuilderGetRequestConfiguration(query_params=query_params = DefinitionsRequestBuilderGetQueryParameters()
query_params['top'] = 100
query_params['skip'] = 0

)
query_params = DefinitionsRequestBuilderGetQueryParameters()
query_params['top'] = 100
query_params['skip'] = 0

)


result = await client.identityGovernance.accessReviews.definitions.get(request_configuration)


```