---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = SessionsRequestBuilderGetRequestConfiguration()

query_params = SessionsRequestBuilderGetQueryParameters()
query_params.expand = ["segments"]

request_config.queryParameters = query_params


result = await client.communications.callRecordsby_id('callRecord-id').sessions.get(request_config)


```