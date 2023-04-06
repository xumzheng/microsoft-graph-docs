---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AccessReviewsRequestBuilderGetRequestConfiguration(
request_config = AccessReviewsRequestBuilderGetRequestConfiguration(query_params=params['filter'] = "businessFlowTemplateId eq '6e4f3d20-c5c3-407f-9695-8460952bcc68'"
params['top'] = 100
params['skip'] = 0
)


result = await client.accessReviews.get(request_config, headers=request_config)


```