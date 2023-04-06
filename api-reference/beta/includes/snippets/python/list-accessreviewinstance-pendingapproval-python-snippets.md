---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = PendingAccessReviewInstancesRequestBuilderGetRequestConfiguration(
request_configuration = PendingAccessReviewInstancesRequestBuilderGetRequestConfiguration(query_params=query_params = PendingAccessReviewInstancesRequestBuilderGetQueryParameters()
query_params['expand'] = ["definition"]
query_params['top'] = 100
query_params['skip'] = 0

)
query_params = PendingAccessReviewInstancesRequestBuilderGetQueryParameters()
query_params['expand'] = ["definition"]
query_params['top'] = 100
query_params['skip'] = 0

)


result = await client.me.pendingAccessReviewInstances.get(request_configuration)


```