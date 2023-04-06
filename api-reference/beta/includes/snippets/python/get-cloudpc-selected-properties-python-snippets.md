---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = CloudPCRequestBuilderGetRequestConfiguration(
request_config = CloudPCRequestBuilderGetRequestConfiguration(query_params=params['select'] = ["id","displayName","imageDisplayName","lastModifiedDateTime","lastRemoteActionResult","lastLoginResult","connectivityResult"]
)


result = await client.deviceManagement.virtualEndpoint.cloudPCs_by_id('cloudPC-id').get(request_config, headers=request_config)


```