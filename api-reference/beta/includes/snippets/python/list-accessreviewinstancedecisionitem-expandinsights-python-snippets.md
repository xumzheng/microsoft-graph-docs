---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = DecisionsRequestBuilderGetRequestConfiguration()

query_params = DecisionsRequestBuilderGetQueryParameters()
query_params.expand = ["insights"]

request_config.queryParameters = query_params


result = await client.identityGovernance.accessReviews.definitions._by_id('accessReviewScheduleDefinition-id').instances._by_id('accessReviewInstance-id').decisions.get(request_config)


```