---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = DefinitionsRequestBuilderGetRequestConfiguration()

query_params = DefinitionsRequestBuilderGetQueryParameters()
query_params.top = 100
query_params.skip = 0

request_config.queryParameters = query_params


result = await client.identityGovernance_accessReviews_definitions.get(request_config)


```