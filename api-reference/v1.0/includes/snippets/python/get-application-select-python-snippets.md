---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ApplicationRequestBuilderGetRequestConfiguration()

query_params = ApplicationRequestBuilderGetQueryParameters()
query_params.select = ["id","appId","displayName","requiredResourceAccess"]

request_config.queryParameters = query_params


result = await client.applications._by_id('application-id').get(request_config)


```