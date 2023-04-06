---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ApplicationRequestBuilderGetRequestConfiguration(
request_config = ApplicationRequestBuilderGetRequestConfiguration(query_params=query_params = ApplicationRequestBuilderGetQueryParameters()
query_params.select = ["id","appId","displayName","requiredResourceAccess"]

)
query_params = ApplicationRequestBuilderGetQueryParameters()
query_params.select = ["id","appId","displayName","requiredResourceAccess"]

)


result = await client.applications_by_id('application-id').get(request_config, headers=request_config)


```