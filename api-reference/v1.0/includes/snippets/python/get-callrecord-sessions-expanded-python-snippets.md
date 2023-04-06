---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = SessionsRequestBuilderGetRequestConfiguration(
request_config = SessionsRequestBuilderGetRequestConfiguration(query_params=query_params = SessionsRequestBuilderGetQueryParameters()
query_params.expand = ["segments"]

)
query_params = SessionsRequestBuilderGetQueryParameters()
query_params.expand = ["segments"]

)


result = await client.communications.callRecords_by_id('callRecord-id').sessions.get(request_config, headers=request_config)


```