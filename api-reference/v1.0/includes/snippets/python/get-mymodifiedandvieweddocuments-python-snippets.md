---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = UsedRequestBuilderGetRequestConfiguration()

query_params = UsedRequestBuilderGetQueryParameters()
query_params.orderby = ["LastUsed/LastAccessedDateTime desc"]

request_config.queryParameters = query_params


result = await client.me.insights.used.get(request_config)


```