---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = DecisionsRequestBuilderGetRequestConfiguration(
request_config = DecisionsRequestBuilderGetRequestConfiguration(query_params=query_params = DecisionsRequestBuilderGetQueryParameters()
query_params.top = 100
query_params.skip = 0

)
query_params = DecisionsRequestBuilderGetQueryParameters()
query_params.top = 100
query_params.skip = 0

)


result = await client.identityGovernance.accessReviews.definitions_by_id('accessReviewScheduleDefinition-id').instances_by_id('accessReviewInstance-id').decisions.get(request_config, headers=request_config)


```