---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = PendingAccessReviewInstancesRequestBuilderGetRequestConfiguration();

query_params = PendingAccessReviewInstancesRequestBuilderGetQueryParameters();
query_params.expand = ["definition"];
query_params.top = 100;
query_params.skip = 0;

request_config.queryParameters = query_params;


result = awaitclient.me().pendingAccessReviewInstances().get(request_config);


```