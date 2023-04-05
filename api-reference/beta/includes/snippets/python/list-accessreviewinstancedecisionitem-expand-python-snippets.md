---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AccessReviewInstanceDecisionItemRequestBuilderGetRequestConfiguration()

query_params = AccessReviewInstanceDecisionItemRequestBuilderGetQueryParameters()
query_params.expand = ["instance($expand=definition)"]

request_config.queryParameters = query_params


result = await client.identityGovernance.accessReviews.decisionsById('accessReviewInstanceDecisionItem-id').get(request_config)


```