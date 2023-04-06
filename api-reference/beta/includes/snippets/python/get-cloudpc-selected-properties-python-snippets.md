---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = CloudPCRequestBuilderGetRequestConfiguration(
request_configuration = CloudPCRequestBuilderGetRequestConfiguration(query_params=query_params = CloudPCRequestBuilderGetQueryParameters()
query_params['select'] = ["id","displayName","imageDisplayName","lastModifiedDateTime","lastRemoteActionResult","lastLoginResult","connectivityResult"]

)
query_params = CloudPCRequestBuilderGetQueryParameters()
query_params['select'] = ["id","displayName","imageDisplayName","lastModifiedDateTime","lastRemoteActionResult","lastLoginResult","connectivityResult"]

)


result = await client.deviceManagement.virtualEndpoint.cloudPCs_by_id('cloudPC-id').get(request_configuration)


```