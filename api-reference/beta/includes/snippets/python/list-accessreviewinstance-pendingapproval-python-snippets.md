---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = PendingAccessReviewInstancesRequestBuilderGetRequestConfiguration(
request_config = PendingAccessReviewInstancesRequestBuilderGetRequestConfiguration(query_params=params['expand'] = ["definition"]
params['top'] = 100
params['skip'] = 0
)


result = await client.me.pendingAccessReviewInstances.get(request_config, headers=request_config)


```