---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = DefinitionsRequestBuilderGetRequestConfiguration(
request_config = DefinitionsRequestBuilderGetRequestConfiguration(query_params=params['filter'] = "contains(scope/microsoft.graph.accessReviewQueryScope/query,%20'./members')"
)


result = await client.identityGovernance.accessReviews.definitions.get(request_config, headers=request_config)


```