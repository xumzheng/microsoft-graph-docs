---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = DefinitionsRequestBuilderGetRequestConfiguration(
request_configuration = DefinitionsRequestBuilderGetRequestConfiguration(query_params=query_params = DefinitionsRequestBuilderGetQueryParameters()
query_params['filter'] = "contains(scope/microsoft.graph.accessReviewQueryScope/query,%20'./members')"

)
query_params = DefinitionsRequestBuilderGetQueryParameters()
query_params['filter'] = "contains(scope/microsoft.graph.accessReviewQueryScope/query,%20'./members')"

)


result = await client.identityGovernance.accessReviews.definitions.get(request_configuration)


```