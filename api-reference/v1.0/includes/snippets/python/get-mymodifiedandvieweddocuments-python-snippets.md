---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = UsedRequestBuilderGetRequestConfiguration(
request_configuration = UsedRequestBuilderGetRequestConfiguration(query_params=query_params = UsedRequestBuilderGetQueryParameters()
query_params['orderby'] = ["LastUsed/LastAccessedDateTime desc"]

)
query_params = UsedRequestBuilderGetQueryParameters()
query_params['orderby'] = ["LastUsed/LastAccessedDateTime desc"]

)


result = await client.me.insights.used.get(request_configuration)


```