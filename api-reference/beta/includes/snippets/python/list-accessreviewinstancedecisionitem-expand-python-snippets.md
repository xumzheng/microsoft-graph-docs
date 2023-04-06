---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AccessReviewInstanceDecisionItemRequestBuilderGetRequestConfiguration(
request_config = AccessReviewInstanceDecisionItemRequestBuilderGetRequestConfiguration(query_params=query_params = AccessReviewInstanceDecisionItemRequestBuilderGetQueryParameters()
query_params.expand = ["instance($expand=definition)"]

)
query_params = AccessReviewInstanceDecisionItemRequestBuilderGetQueryParameters()
query_params.expand = ["instance($expand=definition)"]

)


result = await client.identityGovernance.accessReviews.decisions_by_id('accessReviewInstanceDecisionItem-id').get(request_config, headers=request_config)


```